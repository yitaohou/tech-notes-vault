---
video_id: CyLYY_xb5bQ
url: https://www.youtube.com/watch?v=CyLYY_xb5bQ
title: You Can Learn AI Agent System Design In 19 Min | RAG, Vector Database, Evals,
  Function Calling
channel: Sean‘s AI Stories
published: '2025-08-25'
duration: '19:28'
transcript_origin: subs
tags:
- video
---

# You Can Learn AI Agent System Design In 19 Min | RAG, Vector Database, Evals, Function Calling

摘要: [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag-summary|完整摘要]]

## 知识点

- [[agent-escalation-low-confidence]] — 当 router agent 判断用户情绪非常激烈，或问题复杂程度超出自身处理置信度时，系统需要有机制将该对话转交给人工处理（human-in-the-loop）。（[06:00](https://youtu.be/CyLYY_xb5bQ?t=360)）
- [[agent-specialization]] — 当发现某个 agent 承担的任务过多时，应将其拆分为多个只专注做一件事的更小 agent，以降低出现 hallucination 的风险。（[13:35](https://youtu.be/CyLYY_xb5bQ?t=815)）
- [[agentic-write-actions]] — 退货流程中，planner agent 在确认符合政策后会触发 Shopify API 执行 return，这是一个会对外部系统产生实际改变的 write action。（[14:35](https://youtu.be/CyLYY_xb5bQ?t=875)）
- [[ai-agent-automation-rate-target]] — e-commerce 客服 agent 系统设计目标之一是实现超过70%的对话自动化处理，其余约30%需要人工介入。（[00:00](https://youtu.be/CyLYY_xb5bQ?t=0)）
- [[api-gateway]] — 在 AI 客服 agent 系统中，gateway 需要处理身份认证（如 single sign-on）、PII 隐私保护、rate limiting 以及请求去重检查等前置校验工作。（[06:00](https://youtu.be/CyLYY_xb5bQ?t=360)）
- [[auth-gate-before-processing]] — 系统设计上要求在继续处理任何用户信息之前，必须先完成 authentication，这是请求处理流程的强制前置门控。（[06:00](https://youtu.be/CyLYY_xb5bQ?t=360)）
- [[business-goal-observability-tracking]] — 构建 agentic 系统后必须持续追踪与业务目标对应的指标，例如自动化处理比例达到70%、转人工比例30%、用户满意度高于4.5、响应时间达标，以验证系统是否满足预设目标。（[15:04](https://youtu.be/CyLYY_xb5bQ?t=904)）
- [[chat-history-relational-storage]] — 为了加载用户此前的聊天记录和邮件，AI 客服系统需要从关系型数据库（relational database）中查询这些历史数据。（[06:00](https://youtu.be/CyLYY_xb5bQ?t=360)）
- [[clear-explicit-instructions-strategy]] — 为 return planner agent 编写提示词时需要清楚定义执行顺序（先做各项 check，再触发功能调用）和参数类型，确保 agent 准确理解需要执行的步骤，避免过度简化导致理解偏差。（[13:45](https://youtu.be/CyLYY_xb5bQ?t=825)）
- [[crm-write-back-trigger]] — 如果客户已经在使用外部 CRM 系统，agent 系统设计中还需要加入自动触发器，把处理结果同步写回该 CRM，以保持外部系统的数据一致。（[15:04](https://youtu.be/CyLYY_xb5bQ?t=904)）
- [[customer-satisfaction-score-metric]] — 客服 agent 系统可将 CSAT 评分目标设为高于4.5/5，作为衡量客户满意度的核心指标。（[00:00](https://youtu.be/CyLYY_xb5bQ?t=0)）
- [[customer-service-agent-return-exchange-rules]] — 退换货政策要求产品必须处于良好状态（good condition）才允许退换。（[03:00](https://youtu.be/CyLYY_xb5bQ?t=180)）
- [[deterministic-workflow-planner]] — 对于流程非常固定的任务（如标准退货流程：先判断商品是否符合退货条件，再触发 Stripe 处理退款），可以用确定性规则工作流代替 agent 自主推理，以提升可控性。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
- [[embedding]] — 向量数据库通过 embedding 把每个词或每段文字转换成高维数字向量，本质是把文本内容『数字化』，类似照片被数字化存储后即可通过计算相似度进行搜索。（[03:00](https://youtu.be/CyLYY_xb5bQ?t=180)）
- [[function-calling]] — function calling 的核心思路是预先准备一份很长的工具/函数列表，让 AI agent 在处理任务时自主挑选合适的工具调用。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
- [[guardrails-policy-alignment-check]] — 可以把退货政策文本传给 guardrails 服务，让其对 RAG 检索出的信息做二次比对，判断是否符合公司政策，再决定是否通知 agent 继续执行。（[13:05](https://youtu.be/CyLYY_xb5bQ?t=785)）
- [[human-approval-for-impactful-actions]] — 客服 agent 系统中若退款金额达到或超过某一阈值（如50美元），系统应将决策升级给人工经理审批，而非由 agent 自动执行退款，以模拟真实人工客服的处理流程。（[00:00](https://youtu.be/CyLYY_xb5bQ?t=0)）
- [[human-handoff-triggers]] — 转人工的两种典型触发场景是：用户主动要求转人工，或系统检测到对话中出现强烈负面情绪需要人工提供情感支持。（[03:00](https://youtu.be/CyLYY_xb5bQ?t=180)）
- [[human-in-the-loop-plan-review]] — 在多 agent 客服系统中，可在 router agent 判断请求有效后插入人工审批环节，由人类决定是否批准该请求，以保障整体客户满意度不受影响。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
- [[intent-specific-planner-agent]] — 当 router agent 判定用户意图为退货时，会调用专门的 return planning agent 接手处理后续的退货流程规划。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
- [[knowledge-augmentation-tools]] — 通过集成 Shopify API，agent 可以查询订单当前状态以及退货授权（RMA）信息，必要时也可处理换货动作。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
- [[latency-percentiles-vs-average]] — 客服 agent 系统的响应延迟目标通常按百分位数设定，例如50%的请求响应时间低于1秒、95%的请求响应时间低于2.5秒。（[00:00](https://youtu.be/CyLYY_xb5bQ?t=0)）
- [[model-routing]] — router agent 的核心职责是识别用户请求的意图（如「退货」），并据此将请求分流给对应的下游 planner agent 处理。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
- [[multi-channel-agent-entry-point]] — 设计客服 agent 系统时首先要明确用户会通过哪些渠道触达系统，本例中包括网站聊天（website chat）和邮件（email）两种渠道。（[03:00](https://youtu.be/CyLYY_xb5bQ?t=180)）
- [[p50-latency-target-agent-system]] — 该 AI 客服 agent 系统的一项关键非功能性需求是保证 50% 的用户响应时间在 1 秒以内（p50 latency 小于 1 秒）。（[06:00](https://youtu.be/CyLYY_xb5bQ?t=360)）
- [[planner-agent-tool-selection]] — 针对退货场景，planner agent 会同时选择调用 Shopify 的退货 API 与 Stripe 的支付 API 这两个工具来完成任务。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
- [[planner-context-handback-to-qa-agent]] — 无论任务成功还是失败（例如商品或问题不符合退货政策），planner agent 完成处理后都要把最新状态更新回 Q&A agent，以便 Q&A agent 能实时回应用户。（[15:04](https://youtu.be/CyLYY_xb5bQ?t=904)）
- [[policy-check-gate-before-tool-call]] — return planner agent 会先完成 RAG 政策检索与 guardrails 比对，确认符合政策后才触发具体功能调用（如 Shopify API 处理退货），形成先检查后执行的决策链路。（[14:10](https://youtu.be/CyLYY_xb5bQ?t=850)）
- [[prefer-deterministic-over-agentic]] — 涉及支付等对准确性要求高的场景，更适合用确定性（deterministic）逻辑处理，而非交给 agent 自主判断，减少不必要的 agent 使用能让系统更可靠。（[12:01](https://youtu.be/CyLYY_xb5bQ?t=721)）
- [[qa-agent-central-hub-role]] — 系统中的 Q&A agent 被类比为公司的中枢大脑或 CEO，是唯一直接与原始用户渠道（web chat、email）沟通的 agent，其余专业 agent 都是向它汇报工作结果的组织成员。（[15:04](https://youtu.be/CyLYY_xb5bQ?t=904)）
- [[qa-agent-latency-filler]] — Q&A agent 会在 router agent 思考路由决策的同时，用「让我帮你查一下」之类的话术并展示 thinking process 来回应用户，使对话显得自然流畅，同时为后端处理争取时间。（[06:00](https://youtu.be/CyLYY_xb5bQ?t=360)）
- [[relational-vs-vector-database-storage-choice]] — 客服 agent 系统需要决定聊天历史、交易信息、退货物流信息究竟存储在关系型数据库还是向量数据库中。（[03:00](https://youtu.be/CyLYY_xb5bQ?t=180)）
- [[response-latency-satisfaction-impact]] — 响应时间过长会显著降低客户满意度，这是客服 agent 系统需要设定严格延迟目标（如 p50、p95）的原因。（[00:00](https://youtu.be/CyLYY_xb5bQ?t=0)）
- [[retrieval-augmented-generation]] — RAG 本质是通过语义检索获取大模型本身不掌握的 private data（如公司退货政策），把这些专有信息喂给 AI agent 使用。（[12:39](https://youtu.be/CyLYY_xb5bQ?t=759)）
- [[return-planner-stripe-refund-flow]] — return planner agent 完成退款判定后会调用 Stripe API 发起实际的支付退款，Stripe API 处理完成后返回「payment refund done」的确认信息。（[15:04](https://youtu.be/CyLYY_xb5bQ?t=904)）
- [[return-policy-business-rule]] — 电商退货规则通常包含购买时间限制（如30天内）和商品状态要求（须为良好状态），用于防止 agent 无条件允许任意退货。（[00:00](https://youtu.be/CyLYY_xb5bQ?t=0)）
- [[router-agent]] — router agent 是最先接触用户问题的 agent，负责理解用户意图并据此决定接下来该把对话路由给哪个 agent 处理。（[06:00](https://youtu.be/CyLYY_xb5bQ?t=360)）
- [[router-agent-planner-hierarchy]] — router agent 处于比各专业 planner agent 更高的层级，其职责是判断应该把当前请求路由给哪个具体的 planner（如退货、换货或订单查询）。（[15:04](https://youtu.be/CyLYY_xb5bQ?t=904)）
- [[router-agent-policy-check]] — router agent 在放行请求进入下一步骤前，需要先核实该请求是否符合公司政策。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
- [[scalability-requirement-user-count]] — 设计 agentic 系统时，scalability、每秒请求数（requests per second）、seasonality 等服务端相关的非功能性需求容易被非技术视角忽略，但产品经理最终仍需与工程负责人共同讨论确定这些指标才能让产品具备上生产环境的条件。（[18:05](https://youtu.be/CyLYY_xb5bQ?t=1085)）
- [[seasonality-traffic-peak-planning]] — 设计客服 agent 系统后端时需要评估每秒请求峰值（peak requests per second）及季节性因素，例如黑色星期五、圣诞节等购物高峰期的流量会显著高于平时。（[03:00](https://youtu.be/CyLYY_xb5bQ?t=180)）
- [[system-design-requirement-scoping]] — 设计客服 agent 系统前应先明确功能范围，例如仅聚焦退货（returns）、换货（exchanges）和订单查询（where is my order），排除其他客服场景。（[00:00](https://youtu.be/CyLYY_xb5bQ?t=0)）
- [[vector-database]] — 传统关系型数据表用行列结构存储数据（类似 Excel 表格，每列代表一个 feature，每行代表一条 entry），但像退款政策这类非结构化文本内容（段落或 PDF）不适合这种表格格式，因此需要存入向量数据库。（[03:00](https://youtu.be/CyLYY_xb5bQ?t=180)）
- [[vector-database-rag]] — FAQ、政策文档这类非结构化的段落型数据不易在表格中检索，更适合存入向量数据库并通过语义相似度检索获取相关信息。（[12:20](https://youtu.be/CyLYY_xb5bQ?t=740)）
- [[vector-similarity]] — 文本被转换为向量后，可以通过计算向量之间的相似度来实现语义层面的搜索与比较。（[03:00](https://youtu.be/CyLYY_xb5bQ?t=180)）
- [[write-action-tools]] — 退货流程中可以集成 Stripe API 这类 write action 工具，让 agent 直接发起退款，或为用户购买的替代商品扣款。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
