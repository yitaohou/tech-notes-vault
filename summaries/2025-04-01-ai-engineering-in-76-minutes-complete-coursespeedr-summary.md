---
video_id: JV3pL1_mn2M
title: AI Engineering in 76 Minutes (Complete Course/Speedrun!)
source: '[[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: b1c3cae4a493930db1d4fef1f9eb66844c57de6b0e6d5ab88651b4972f2082f9
  schema_version: 1
  model: sonnet
  generated_at: '2026-08-26T19:41:00+00:00'
---

## 一句话总结

这是一门 76 分钟的 AI engineering 速成课，系统串联了从 [[foundation-model]] 的训练原理、[[post-training]]、evaluation、[[prompt-engineering]]、[[retrieval-augmented-generation]]、[[agent-definition|agent]]、[[fine-tuning]]、到 [[inference-optimization]] 与生产级应用架构的完整技术栈，核心主张是：AI engineering 的难点已经从"训练模型"转移到"如何评估、适配和部署已有的 foundation model"（[[model-selection-ai-engineering]]）。

## 核心内容

### Foundation model 的由来与内在局限

[[ai-engineering]] 兴起的原因是模型能力大幅提升、开发门槛大幅降低，其工作方式是基于已有 [[foundation-model]] 做 adaptation 而非重新训练（00:00）。Foundation model 的知识边界完全取决于训练数据，而大多数模型使用 [[web-crawled-training-data-issues|网络爬取数据]] 训练，这类数据混杂 clickbait、错误信息乃至假新闻（00:00）。数据分布本身也有偏差：[[training-data-language-distribution-skew]] 显示约一半训练数据是英语，[[training-data-domain-distribution-skew]] 显示主题偏向商业科技类内容，这催生了 [[specialized-language-domain-models|专用语言/领域模型]] 的需求。GPT-2 用 Reddit upvote 数过滤数据是应对质量问题的典型案例（[[gpt2-reddit-filter-example]]，00:00）。模型扩张面临两大瓶颈：[[training-data-scarcity-bottleneck|高质量数据即将枯竭]]和 [[energy-bottleneck-data-centers|数据中心能耗已占全球电力1-2%]]（06:00），应对方式包括转向 [[ai-generated-content-training-degradation|AI生成数据]]（有性能退化风险）或 [[proprietary-data-access-solution|获取专有数据]]。

架构上，[[transformer-architecture]] 通过 [[attention-mechanism]] 解决了 [[encoder-decoder-architecture|传统 encoder-decoder]] 的 [[sequential-processing-bottleneck|串行瓶颈]]：[[query-key-value-vectors|Q/K/V 向量]]配合 [[multi-head-attention|多头机制]]（Llama 2 7B 有 32 个头，03:00），推理分 [[transformer-prefill-decode|prefill 与 decode]] 两阶段。[[chinchilla-scaling-law]] 指出训练 token 数约为参数量的 20 倍是最优配比，但 [[diminishing-returns-model-improvement|边际收益递减]]明显：错误率从 3% 降到 2% 可能要多一个数量级的资源投入（03:00）。

### Post-training 与采样带来的概率性本质

预训练模型有两大问题：面向补全而非对话、输出可能事实错误（[[pretrained-foundation-model-issues]]）。[[post-training]] 通过 [[supervised-fine-tuning]]（教会对话格式）和 [[preference-fine-tuning]]（[[rlhf]] 或更新的 [[dpo]]，也可用 [[best-of-n-sampling]] 跳过强化学习）解决（06:00）。模型输出本质是 [[probabilistic-output-nature|概率分布]]，通过 [[greedy-sampling]]、[[temperature-sampling]]、[[top-k-sampling]]、[[top-p-sampling]] 等策略采样，这也是 [[hallucination]] 现象和 [[ai-evaluation-importance|evaluation 重要性]]的根源（06:00）。

### Evaluation：AI engineering 中被低估却最复杂的环节

评估天然复杂（[[evaluation-inherent-complexity]]），因为 [[foundation-model-black-box|模型是黑盒]]、任务常常是 [[open-ended-task-evaluation|开放式]]的，还要面对 [[benchmark-saturation|基准饱和]]与 [[capability-discovery-evaluation|能力发现]]的挑战（09:01）。技术上，[[cross-entropy]]、[[entropy-information-theory]]、[[perplexity]] 是语言建模的基础指标，也可用于 [[perplexity-contamination-signal|检测数据污染]]；[[exact-evaluation]]/[[exact-match-evaluation]] 适用于确定性答案，[[functional-correctness]]（如代码的 [[execution-accuracy]]）是黄金标准。评估方法上，[[reference-based-evaluation]]（[[lexical-similarity-evaluation]]、[[semantic-similarity-evaluation]]）与 [[llm-as-a-judge]] 是主流，后者能做打分、比较、选优三种用途，但存在 [[ai-judge-bias|self/position/verbosity 三种偏见]]和 [[ai-judge-limitations|不稳定性]]（12:01），[[ai-judge-prompt-design|提示词设计]]需包含任务、标准、评分体系。

评估流程需要检验自身可靠性：[[bootstrap-evaluation-reliability-test]]、[[evaluation-pipeline-reliability-checks]]、[[data-slice-evaluation|分群体评估]]避免 [[simpsons-paradox-model-evaluation|辛普森悖论]]（21:01）。生产环境中应采用 [[mixed-evaluation-method-strategy|混合策略]]（全量跑便宜方法+抽样跑昂贵方法）并保留 [[human-evaluation-in-production|人工评估]]。

### 模型选型：两步流程与开源之争

[[model-selection-workflow]] 分四步：[[hard-attributes-model-selection|硬性属性]]过滤 → 公开 [[benchmark-selection-for-model-narrowing|benchmark 缩小候选]] → 自建评估选出最佳 → 生产监控（15:01）。需警惕 [[data-contamination|数据污染]]、[[public-leaderboard-aggregation-challenges|排行榜聚合陷阱]]。[[open-weight-model]] 与 [[open-model-full-definition|真正开源模型]]、[[open-source-model-definition-debate|定义之争]]需分清；是否 [[model-hosting-vs-api-decision|自托管还是用 API]]取决于 [[data-privacy-model-hosting-factor|隐私]]、[[data-lineage-copyright-risk|版权风险]]、[[api-provider-control-risk|控制权风险]]等（18:01）。

### 模型适配三级火箭：Prompting → RAG → Fine-tuning

[[prompting-rag-finetuning-escalation]] 是核心决策框架（45:04）：先用 [[prompt-engineering]] 榨干效果（需要 [[prompt-engineering-requires-rigor|实验严谨性]]，包含 [[system-prompt-vs-user-prompt|system/user prompt]]、[[in-context-learning|in-context learning]]、[[chain-of-thought-prompting|CoT]]等技巧，24:02-27:02）；若因缺信息失败则用 [[retrieval-augmented-generation|RAG]]（[[rag-retriever|retriever 负责 indexing 和 querying]]，[[term-based-retrieval|term-based]] vs [[embedding-based-retrieval|embedding-based]]检索，[[chunk-size-tradeoff|chunking 权衡]]，30:02-33:02）；若是行为类问题则用 [[fine-tuning]]。

[[agent-definition|Agent]] 是比 RAG 更主动的模式，通过 [[knowledge-augmentation-tools]]、[[capability-extension-tools]]、[[write-action-tools]] 三类工具与环境交互，但存在 [[agent-compounding-error-risk|复合误差风险]]（36:03）。[[agent-system-four-pillars|Agent 四大支柱]]是 RAG、工具、[[plan-execution-decoupling|规划]]和 [[agent-memory-system|记忆系统]]（42:04）。

Fine-tuning 方面，[[fine-tuning-memory-requirements|内存需求远高于推理]]，因为需要 [[backpropagation]]；[[parameter-efficient-fine-tuning|PEFT]]（尤其 [[lora]]）通过冻结大部分参数大幅降低成本，且 [[lora-inference-merge|不增加推理延迟]]（45:04-48:04）。[[data-centric-ai|数据中心范式]]强调训练数据质量（[[training-data-quality-factors]]涵盖 coverage、consistency、relevance 等六个维度）比模型架构更能带来差异化竞争力（[[data-centric-competitive-advantage]]，51:04-57:04）。

### 推理优化与生产架构

推理性能受 [[compute-bound-bottleneck]] 或 [[memory-bandwidth-bound-bottleneck|内存带宽瓶颈]]限制，[[autoregressive-inference-memory-bound|自回归 LLM 通常是后者]]（60:04）。关键指标是 [[inference-latency|latency]]（[[total-latency-formula|TTFT+TPOT×token数]]）与 [[inference-throughput|throughput]]，二者存在 [[latency-throughput-tradeoff|权衡]]。优化技术分层：模型压缩（[[quantization]]、[[pruning-model]]、[[knowledge-distillation]]）、解码技巧（[[speculative-decoding]]）、[[request-batching|batching]]、[[model-parallelism|并行化]]（[[tensor-parallelism]]等），最具性价比的是 [[inference-optimization-technique-prioritization|quantization、tensor parallelism、replica parallelism、attention优化]]（66:06）。

最后，[[ai-app-architecture-maturity-stages|应用架构成熟路径]]依次是：加强 [[context-construction-feature-engineering|上下文构建]] → 加 [[input-output-guardrails|guardrails]] → 引入 [[model-routing]]/[[model-gateway]] → [[inference-caching|缓存优化]] → 复杂逻辑与 [[agentic-write-actions|写操作]]（69:07-72:08）。[[ai-system-observability|Observability]]（而非仅 [[ai-system-monitoring|monitoring]]）和 [[user-feedback-competitive-advantage|用户反馈]]是持续改进的关键，但 [[complexity-should-serve-purpose|复杂度必须服务于明确目的]]（75:08）。

## 值得记住的细节

- 00:00 GPT-2 训练数据仅用获得至少 3 个 upvote 的 Reddit 链接过滤质量。
- 03:00 Llama 2 7B 有 32 个 attention heads；Chinchilla law 建议训练 token 数约为参数量的 20 倍（30 亿参数模型需约 600 亿 token）。
- 06:00 top-K 常用范围 50-500；top-P 常用阈值如 0.9；temperature 高温 0.7-1，低温接近 0。
- 12:01 AI judge 有 self bias、position bias、verbosity bias 三种偏见，可用随机化答案顺序缓解但增加成本。
- 18:01 OpenAI Evals 可运行约 500 个现有 benchmark。
- 21:01 客服场景中 factual consistency 从 80%→90% 可能对应自动化处理率从 30%→50%。
- 24:02 GPT-4 偏好任务描述放开头，Llama 3 偏好放结尾。
- 45:04 130 亿参数模型用 32-bit 存储约需 52GB，降到 16-bit 约需 26GB；Llama 2 若误用 fp16（而非训练时的 bf16）会导致输出质量显著变差。
- 51:04 prompt loss weight 默认值通常为 10%；数百万条数据用 1-2 个 epoch，数千条数据可能需 4-10 个 epoch。
- 54:04 OpenAI 微调指南发现：约 100 条样本时更强 base model 微调效果更好；约 55 万条样本时各模型表现趋同。建议先用约 50 条精心制作样本测试效果。
- 60:04 自回归模型总延迟 = TTFT + TPOT × 输出 token 数。
- 63:05 CPU 高端约 64 个核心，GPU 有数千个更小核心，专为并行矩阵乘法优化。
- 72:08 Observability 三大指标：MTTD、MTTR、CFR。

## 这个视频适合谁 / 可以跳过什么

适合：想要一次性建立 AI engineering 全景知识框架的工程师/PM，尤其是需要理解"何时用 prompting、何时用 RAG、何时该 fine-tuning"这类决策逻辑的人，以及需要设计生产级评估体系或推理优化方案的实践者。

可以跳过：如果只关心某个细分主题（例如只想学 RAG 或只想学 fine-tuning 超参数），可以直接跳到对应时间段，无需从头看起，因为各节相对独立；对已经熟悉 Transformer 内部结构（attention、Q/K/V）的观众，00:00-06:00 的架构基础部分可以快进。
