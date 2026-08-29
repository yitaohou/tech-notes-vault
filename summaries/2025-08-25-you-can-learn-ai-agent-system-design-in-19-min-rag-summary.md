---
video_id: CyLYY_xb5bQ
title: You Can Learn AI Agent System Design In 19 Min | RAG, Vector Database, Evals,
  Function Calling
source: '[[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: 7488de66038f77fdde7d08120bdd8b066755f1ecdde11f3820a8f7b9d826be7c
  schema_version: 1
  model: sonnet
  generated_at: '2026-08-27T01:18:46+00:00'
---

## 一句话总结

这是一份针对电商客服 AI agent 系统的端到端 system design 讲解，从需求范围界定、多渠道接入、[[router-agent]]/[[planner-agent-tool-selection|planner agent]] 分层架构，到 [[retrieval-augmented-generation|RAG]]、[[guardrails-policy-alignment-check|guardrails]]、[[agentic-write-actions|write action]] 落地，再到业务指标追踪，完整展示了如何在 19 分钟内把一个"退货/换货/订单查询"客服 agent 从需求文档做到可上线架构（00:00-18:05）。

## 核心内容

### 从业务指标反推系统设计需求

设计任何 agent 系统前，应先做 [[system-design-requirement-scoping|需求范围界定]]，明确本次只处理退货（returns）、换货（exchanges）、订单查询（where is my order）三类场景（00:00）。围绕这个范围定义可量化的业务目标：[[ai-agent-automation-rate-target|自动化率目标]]设为超过 70%，剩余约 30% 走 [[human-handoff-triggers|人工介入]]；[[customer-satisfaction-score-metric|CSAT 目标]]设为高于 4.5/5；[[response-latency-satisfaction-impact|响应延迟会直接影响满意度]]，因此按 [[latency-percentiles-vs-average|百分位数]]设定延迟目标：[[p50-latency-target-agent-system|p50 < 1 秒]]，p95 < 2.5 秒（00:00）。业务规则层面，[[return-policy-business-rule|退货政策]]限定 30 天内、商品须为良好状态，且已拆封食品等品类直接排除在退货范围外（00:00, 03:00，见 [[customer-service-agent-return-exchange-rules]]）；涉及金额较大的退款（如 ≥$50）需要 [[human-approval-for-impactful-actions|人工经理审批]]而非 agent 自动执行，模拟真实客服流程（00:00）。后端容量规划上还要评估 [[scalability-requirement-user-count|并发用户规模]]与 [[seasonality-traffic-peak-planning|季节性流量峰值]]（如黑五、圣诞），这类非功能性需求容易被产品视角忽略，需要 PM 与工程负责人共同拍板（03:00, 18:05）。

### 数据存储的选择：关系型 vs 向量数据库

系统要决定聊天记录、交易信息、物流信息该放关系型数据库还是向量数据库（[[relational-vs-vector-database-storage-choice]]，03:00）。结构化数据（如交易记录）适合传统行列式关系表；而像退货政策这种非结构化的段落/PDF 文本则不适合表格存储，需要用 [[vector-database|向量数据库]]。其原理是通过 [[embedding|embedding]] 把文字数字化为高维向量（类比照片被数字化后可检索），再用 [[vector-similarity|向量相似度]]做语义搜索（03:00）。这一存储选择直接决定了后续 [[vector-database-rag|RAG]] 检索能否工作：FAQ、政策文档等非结构化内容存入向量库后，通过语义相似度检索获取相关片段（12:20），而 [[retrieval-augmented-generation|RAG]] 的本质就是把大模型本身不掌握的私有数据（如公司退货政策）检索出来喂给 agent 使用（12:39）。

### 请求入口与路由：从 gateway 到 router agent

用户可能通过 [[multi-channel-agent-entry-point|多渠道]]（网站聊天、邮件）进入系统（03:00）。请求首先经过 [[api-gateway|API gateway]]，处理 SSO 认证、PII 保护、rate limiting、去重等前置工作（06:00），且系统设计强制要求 [[auth-gate-before-processing|先认证后处理]]（06:00）。认证通过后系统从 [[chat-history-relational-storage|关系型数据库]]加载用户历史聊天/邮件记录（06:00）。之后请求交给 [[router-agent|router agent]]，它是第一个接触用户问题的 agent，通过 [[model-routing|意图识别]]判断该把请求路由给哪个下游 planner（如退货、换货、查订单）（06:00, 09:01）。为了让等待过程不显得生硬，[[qa-agent-latency-filler|Q&A agent]]会用"让我帮你查一下"之类话术并展示 thinking process 来做延迟填充（06:00）。若 router agent 判断情绪激烈或问题复杂度超出置信度，则触发 [[agent-escalation-low-confidence|低置信度升级]]转人工（06:00），这也呼应了 [[human-in-the-loop-plan-review|人工审批环节]]：在 router agent 判定请求有效后插入人工决策点以保障满意度（09:01）；同时 router agent 本身也要做 [[router-agent-policy-check|政策核验]]，确认请求符合公司政策才放行（09:01）。整体上 [[router-agent-planner-hierarchy|router agent 处于比各专业 planner 更高的层级]]，只负责分流决策（15:04）。

### Planner agent 与工具调用：deterministic 优先，agent 按需拆分

一旦意图确定为"退货"，router agent 会调用专门的 [[intent-specific-planner-agent|return planning agent]]（09:01）。这里体现 [[function-calling|function calling]]的核心思路：预先准备一份工具列表，让 agent 自主挑选调用（09:01）。具体到退货场景，planner 会用到多类工具：[[knowledge-augmentation-tools|知识增强类]]工具如 Shopify API 查订单状态和 RMA 信息、3PL API 查物流位置回答"我的订单在哪"（09:01）；[[write-action-tools|写操作类]]工具如 Stripe API 发起退款/扣款、CRM API 读写 deal 和 ticket（09:01, 18:05）。[[planner-agent-tool-selection|针对退货场景]]，planner 会同时选择 Shopify 退货 API 与 Stripe 支付 API 两个工具协同完成任务（09:01）。

但视频强调并非所有流程都要交给 agent 自主推理：像退货这种流程非常固定的任务（先判断是否符合条件，再触发 Stripe 退款），可以用 [[deterministic-workflow-planner|确定性规则工作流]]代替 agent 推理，提升可控性（09:01）；尤其是支付这类对准确性要求极高的场景，更应该 [[prefer-deterministic-over-agentic|优先用确定性逻辑而非 agentic 逻辑]]，减少不必要的 agent 使用能让系统更可靠（12:01）。当发现某个 agent 承担任务过多时，应该做 [[agent-specialization|agent 拆分专精]]，把它拆成多个只做一件事的小 agent，以降低 hallucination 风险（13:35）。写 prompt 时也要用 [[clear-explicit-instructions-strategy|清晰明确的指令]]，明确执行顺序（先 check 再 function call）和参数类型，避免过度简化导致理解偏差（13:45）。

### 政策校验与写操作的执行链路

return planner agent 的执行顺序是：先做 RAG 检索政策 + [[guardrails-policy-alignment-check|guardrails 二次比对]]，确认是否符合公司政策（13:05），这构成了 [[policy-check-gate-before-tool-call|先检查后执行]]的决策链路（14:10）。确认合规后才触发 [[agentic-write-actions|write action]]：调用 Shopify API 执行 return（14:35），或调用 [[return-planner-stripe-refund-flow|Stripe API 发起退款]]，Stripe 处理完返回"payment refund done"确认（15:04）。无论退货流程成功还是因不符合政策而失败，planner agent 都要做 [[planner-context-handback-to-qa-agent|状态回传]]，把最新结果更新回 Q&A agent（15:04）。这里 [[qa-agent-central-hub-role|Q&A agent 的中枢角色]]被类比为公司 CEO：它是唯一直接对接原始用户渠道（web chat/email）的 agent，其余专业 agent 都像向它汇报工作的团队成员（15:04）。如果客户本身在用外部 CRM，系统还需加 [[crm-write-back-trigger|CRM 写回触发器]]，把处理结果自动同步过去，保持外部系统数据一致（15:04）。

### 上线后：持续追踪业务目标

系统搭建完成后，必须持续做 [[business-goal-observability-tracking|业务目标可观测性追踪]]：自动化率是否达到 70%、转人工比例是否维持 30%、CSAT 是否高于 4.5、延迟指标是否达标，用这些指标验证系统是否真正满足最初设定的设计目标（15:04），形成从需求设定到上线验证的闭环。

## 值得记住的细节

- 自动化处理目标：>70%，人工介入约 30%（00:00，[[ai-agent-automation-rate-target]]）
- CSAT 目标：>4.5/5（00:00，[[customer-satisfaction-score-metric]]）
- 延迟目标：p50 < 1 秒，p95 < 2.5 秒（00:00, 06:00，[[p50-latency-target-agent-system]]）
- 退款金额 ≥$50 需人工经理审批，不由 agent 自动执行（00:00，[[human-approval-for-impactful-actions]]）
- 退货政策规则：30 天内 + 商品良好状态；已拆封食品等品类直接排除（00:00, 03:00）
- 转人工两大触发条件：用户主动要求 / 检测到强烈负面情绪（03:00，[[human-handoff-triggers]]）
- 涉及支付等高准确性场景优先用 deterministic 逻辑而非 agentic 逻辑（12:01，[[prefer-deterministic-over-agentic]]）
- return planner 的固定执行顺序：RAG 政策检索 → guardrails 比对 → 通过后才触发 function call（如 Shopify/Stripe API）（13:05-14:35）
- 退货工具组合：Shopify API（订单状态/RMA/换货）+ Stripe API（退款/扣款）+ 3PL API（物流查询）+ CRM API（deal/ticket 读写）（09:01, 18:05）
- Q&A agent 是唯一直接对接用户渠道的 agent，其余 planner 都向它回传状态（15:04）

## 这个视频适合谁 / 可以跳过什么

适合：正在准备 AI/agent 相关 system design 面试的工程师或 PM、想了解 RAG、向量数据库、function calling、多 agent 分层架构如何在真实电商客服场景落地的人，以及需要理解"何时该用 agent、何时该用确定性规则"这类工程取舍的读者。可以跳过：如果你已经熟悉 RAG 和向量数据库的基本原理（03:00 段落对 embedding/向量相似度的科普讲解可跳过），或者只关心业务指标设定而不关心底层架构细节，可以直接看"核心内容"中的指标部分和最后的 observability 小节即可。
