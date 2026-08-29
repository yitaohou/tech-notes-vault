---
video_id: z_F0z7wF5XU
title: AI自我递归改进先要靠Harness工程 | Lilian Weng最新长文 | 反馈循环 | 三个设计模式 | 核心智能 | ACE | MCE |
  Meta-Harness | STOP
source: '[[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: 30175b3e59d39a388b41229bcd0c5b9447305ce1f50feae57f4fd5de03eec794
  schema_version: 1
  model: sonnet
  generated_at: '2026-08-26T19:50:28+00:00'
---

## 一句话总结

Lilian Weng 的这篇长文认为，AI 的递归自我改进短期内不太可能从模型直接改写权重开始，而更现实的路径是 [[harness-engineering|Harness 工程]]——不断优化包裹在模型外部、负责编排上下文、工具调用、工作流和评估的整套系统；文章通过 ACE、Meta-Harness、Self-Harness、DGM、STOP、SIA 等一系列案例，梳理了 Harness 从人工设计走向自动搜索、进而催生元层级优化的演化路径，并指出评估器薄弱、多样性坍塌、奖励黑客等尚未解决的核心瓶颈。

## 核心内容

### 什么是 Harness，为什么它重要

早期业界常把 [[agent-definition|Agent]] 定义为「大模型 + 记忆 + 工具 + 规划 + 行动」，而 [[harness-engineering|Harness 工程]] 在此基础上新增了工作流设计、评估、权限控制和持久状态管理，重心从写提示词模板转向运行时和软件系统设计（00:00）。Claude Code、Codex 这类成功编码 Agent 产品的核心竞争力很大程度上来自成熟的 Harness 设计（00:00）。Harness 的定位类似操作系统：把复杂逻辑封装在内部、对外保持简洁接口，未来配置和工具接口协议大概率会走向标准化（00:00）。其设计原则是尽量简单通用以保证泛化性，这借鉴了软件工程实践、也能复用模型预训练中学到的知识（00:00）。翁荔认为，连接原始模型与真实应用场景的部署系统（harness）重要性可能不亚于模型本身的原生智能（00:00），这也呼应了 [[recursive-self-improvement-harness-vs-intelligence-debate|Harness 层与核心智能孰重孰轻的争论]]——长期占比难以预判，但近期的自我改进路径大概率不会从模型直接改写权重开始（06:04）。

递归自我改进这一概念并不新：I·J·Good 在 1965 年提出「超智能机器」，Eliezer Yudkowsky 于 2008 年正式用 [[recursive-self-improvement|递归自我改进]] 描述 AI 用当前智能改进「产生智能」这一机制本身的反馈循环（00:00）。它可能有两种形式：模型直接改写自身权重，或模型改进自己的训练流水线和部署系统从而催生更强的下一代模型（00:00）。

### 三个核心设计模式与编码 Agent 的工具基础

Harness 反复出现三个设计模式。第一个是 [[harness-workflow-automation-pattern|工作流自动化]]，即给模型定义一套可操作、可测试、可迭代的工作流，[[karpathy-autoresearch|Karpathy 的 autoresearch]] 是一个很干净的例子（00:00）。第二个是 [[harness-goal-directed-loop-pattern|目标导向循环]]，与静态提示词模板不同，模型在运行时持续分析自己的执行轨迹和失败案例来迭代推进任务，遇到描述不清晰时会主动向用户确认而非自行猜测（03:03）。第三个是 [[subagent-background-task-pattern|子agent与后台任务模式]]，用于同时验证多个假设、并行跑实验或隔离子任务以避免污染主上下文，配合一个 [[lightweight-process-manager|轻量进程管理器]] 启动任务、查看日志、取消失败运行并合并结果（03:03）。这里的关键是 [[observable-parallel-process-requirement|可观测性要求]]：子 agent 的输出如果只存在临时聊天上下文里很快会失效，必须存成文件、日志、状态记录才能支持中断恢复和基于完整历史的推理（03:03）。

[[coding-agent-harness-convergence|主流编码 agent 的通用循环]] 已趋于收敛：观察仓库、规划、搜索读取文件、编辑打补丁写测试、运行检查错误，循环往复，如同人类用 IDE 开发（03:03）。对应的 [[coding-agent-toolset|通用工具集]] 包括文件系统操作、Shell 执行、LSP/Git 等开发工具，以及 MCP、技能包、网页搜索等外部上下文工具（03:03）。由于长周期运行产生的日志、diff、论文摘要等产物很快会超出上下文窗口，[[file-system-persistent-memory|用文件系统持久化记忆]] 就成为必要手段，且这种方式能天然随核心模型能力提升而变强（03:03）。

### 上下文工程的自我演化：ACE 与 MCE

[[agentic-context-engineering-ace|ACE]] 不把上下文当成越堆越长的提示词，而是当成一本不断演化、带标识符的要点式操作手册（06:04）。它由三个角色组成（[[ace-generator-reflector-curator-roles|Generator/Reflector/Curator]]）：Generator 生成任务轨迹，Reflector 从成败轨迹中提炼洞见，Curator 用增量条目更新结构化上下文（06:04）。为避免上下文崩塌和简洁性偏差，[[ace-curator-incremental-bullet-design|Curator 采用增量式要点设计]]，不重写整段提示词，而是通过确定性逻辑合并、定期精简去重（06:04）。不过 [[ace-self-managed-memory-limitation|ACE 的自我管理仍有局限]]：更新规则和整体工作流依然是人工设计的（06:04）。

[[context-management-layer|上下文管理层]] 的作用是构建更结构化精简的上下文并管理持久状态，防止任务周期变长时上下文体量失控（06:04），尽管长上下文能力一直在进步，但现阶段 [[long-context-context-engineering-interplay|长上下文表现和上下文工程仍紧密交织]]（06:04）。在此基础上，[[meta-context-engineering-mce|MCE]] 把上下文管理机制本身与上下文内容分离，是更进一步的自我改进方向（06:04）。[[mce-framework|MCE 框架]] 分为元层级（技能演化）和基础层级（针对给定技能的上下文优化）（09:06），对应 [[mce-two-level-optimization|双层优化]]：内层在给定技能下搜索最优上下文，外层在验证集上挑选最佳技能（09:06）。这里 [[skill-as-context-function|技能被定义为上下文函数]]，包含静态组件（提示词、知识库等）和动态算子（搜索、筛选、格式化等）（09:06），在实现上就是专门目录里的一堆文件（[[context-function-file-implementation]]，09:06）。系统维护一个 [[skill-database|技能数据库]] 记录历史技能及其评估指标（09:06），[[meta-agent-skill-crossover|元级 Agent 基于历史技能交叉生成新技能]]，交给基础层执行并优化（09:06），两级都共享同一套标准编码 Agent 工具（[[meta-base-level-shared-tooling]]，09:06）。

这一系列进展体现了 [[harness-meta-methodology-evolution|Harness 向元方法论演化]] 的趋势：改进的是获取答案的机制本身，而非答案内容（06:04）。翁荔总结了 [[harness-optimization-target-escalation|被优化对象的逐步升级]]：从指令提示词，到结构化上下文，到工作流，到 Harness 代码，最终到优化器本身的代码（06:04），[[harness-as-optimization-target|Harness 本身正在成为被优化的目标]]，人工启发式规则逐渐减少、通用机制逐渐增多（06:04）。类比 [[prompt-engineering-decline-precedent|提示工程重要性的下降]]——随指令微调和推理能力提升，手动提示技巧变得不那么重要，但定义目标、约束、上下文和评估的需求从未消失（06:04）；同理，[[stronger-model-prevents-harness-overengineering|更强的模型能避免 Harness 过度工程化]]（06:04），长期看 [[harness-improvement-internalization|很多 Harness 改进会被内化进核心模型]]，但外部上下文和工具接口层预计会一直存在（06:04）。[[mature-harness-automated-research-loop|成熟的 Harness 能支撑自动研究闭环]]，反过来推动模型自我改进（06:04）。

### 自动化研究系统与把 Harness 设计变成搜索问题

[[ai-scientist-system|AI Scientist 系统]] 搭建了从提出想法、写代码跑实验、分析结果、写论文到同行评审的完整自动研究流水线（09:06）。[[scientistone|ScientistOne]] 把可验证性作为核心约束，要求每个论断都能追溯到证据来源（09:06）。[[autodata-agent|AutodataAgent]] 定位为自动数据科学家，由挑战者、弱求解器、强求解器、验证裁判四个角色组成的主 Agent 管理，合成难度恰当的任务（09:06）。这些例子说明 [[manual-harness-design-era|早期 Harness 工作流依赖领域专家手工设计]]的时代正在被自动搜索方法取代（09:06）。

[[meta-harness|Meta-Harness]] 直接把优化对象对准 Harness 本身——决定信息如何存储、检索、呈现给模型的整套代码（09:06）。其 [[meta-harness-outer-loop|外层循环]]：初始化一批候选、在文件系统存下代码/分数/轨迹，每轮由 [[meta-harness-proposer-agent|提案者 Agent]]（本身是编码 Agent，用 grep/cat 读历史记录而非塞进提示词）生成新候选，验证合格后加入池子，最终输出帕累托最优方案（09:06）。每个候选对应文件系统里一个含源码、评分、轨迹的目录（[[harness-candidate-directory-structure]]，09:06）。在 [[terminalbench-2|TerminalBench-2]] 基准上，Meta-Harness 优化方案超过了很多人工强基线（09:06），这说明一旦 [[harness-design-as-search-space|Harness 设计变成可执行搜索空间]]，强编码 Agent 就能探索和人类工程师完全一样的设计空间（09:06）。

这一思路延伸到更早的 [[agentic-workflow-design-as-search-problem|把工作流设计当作搜索问题]]：[[ads-automated-design-agentic-systems|ADAS]] 让元 agent 参考存档中现有方案迭代生成新 agent 代码（12:08）；[[aflow-agentic-workflow-search|AFlow]] 用分数与探索混合策略选择节点、迭代修改工作流，在问答、代码、数学任务上超过人工设计和 ADAS（12:08）。核心逻辑是：若模型能直接优化执行 agent 的代码，触及的设计空间远比手写提示词大得多（[[harness-as-code]]，12:08）。[[self-taught-optimizer-stop|STOP]] 定义「元效用」并递归地用上一代优化器优化自身，自主发现遗传算法、模拟退火、束搜索等多种优化策略（12:08），但 [[stop-self-improving-optimizer|若基础模型换成能力更弱的 GPT-3.5 或 Mixtral，性能反而随迭代下降]]，说明基础模型能力必须足够强才能真正改进机制本身（15:08）。相对地，[[challenger-solver-verifier-loop|挑战者-求解者-验证者循环]]生成的合成数据只用来微调弱模型、不迭代改进强模型，更接近间接知识蒸馏，自我改进属性并不强（12:08）。

### 进化搜索家族：从 AlphaEvolve 到 DGM 再到 SIA

[[evolutionary-search|进化搜索]] 特别适合搜索空间大、形状不规则、难以梯度优化但评估容易的场景，Harness 搜索恰好同时符合（15:08）。[[alphaevolve|AlphaEvolve]] 维护候选程序池，用参数冻结的大模型生成 diff 补丁改进程序，反复评估、保留成功个体（15:08、18:11）；其 [[alphaevolve-prompt-design|提示词设计]]包含父程序、运行结果、指令和元信息，需改进区域会专门标出（18:11），且 [[alphaevolve-meta-prompt-coevolution|元提示词会与指令、上下文一起随建议共同进化]]（18:11）。[[gepa|GEPA]] 将反思式提示词与进化搜索结合，靠对试错轨迹的自然语言反思生成更新方向（15:08）。[[promptbreeder|Promptbreeder]] 通过丰富变异操作进化任务特定提示词，连变异指令本身也随进化演化（15:08）。[[theta-evolve|ThetaEvolve]] 把进化搜索、强化学习和上下文学习结合，是 AlphaEvolve 的后续变种（18:11）。[[shinka-evolve|ShinkaEvolve]] 新增三个组件提升采样效率：[[shinka-evolve-parent-sampling|父代采样平衡性能排名与后代数量]]、[[shinka-evolve-novelty-rejection|基于嵌入相似度的新颖性拒绝采样]]、[[shinka-evolve-meta-scratchpad|元草稿本总结成功变异模式]]（18:11）。

[[darwin-godel-machine|达尔文哥德尔机（DGM）]] 明确把优化目标对准可编辑的 Harness 代码仓库，让编码 agent 修改自己的 Harness（18:11）。其 [[dgm-workflow|工作流]] 从单个 agent 起步，按 [[dgm-parent-selection|性能正比、后代数量反比的概率]]选父 agent，令其检查日志并提出对自身 Harness 的改进（18:11），[[dgm-code-editing-tools|代码编辑仅靠 bash 和文件编辑器两个基础工具]]实现（18:11）。[[dgm-experiment-results|实验结果]]以 Claude 3.5 Sonnet 为基础模型，从简单初始配置进化出的 agent 在 SWE-bench Verified 和 Polyglot 上追平甚至超过人工设计的 agent（18:11）。但 [[dgm-limitations|DGM 类方法有明显局限]]：只适合能自动评估、适应度容易量化的场景，对评估慢、标准模糊、依赖主观判断的领域难以适用（18:11），本质上 [[dgm-fixed-model-harness-evolution|DGM 是固定模型下的 Harness 进化]]，不涉及权重更新（18:11）。[[hyperagents|Hyperagents]] 在 DGM 基础上引入元 agent，专门控制如何修改现有任务 agent 以及生成新 agent（18:11）。

以上方法都停留在 [[harness-vs-weight-update-recursive-improvement|Harness 层面优化非参数系统]]，而完整的递归自我改进也可以让模型同时更新权重（18:11）。[[sia-self-improving-agent|SIA]] 就是把 Harness 改进和权重更新放进同一循环的早期尝试：[[sia-agent-roles|元 agent 提出初始 Harness，任务特定 agent 执行任务，反馈 agent 决定下一步更新 Harness 还是权重]]（18:11），[[sia-lora-weight-update|权重更新采用 LoRA 方式通过强化学习完成]]（18:11）。但翁荔提醒 [[sia-confounding-factors|该实验存在混淆因素]]，需谨慎解读（18:11），具体表现为 [[meta-agent-feedback-agent-task-agent-architecture|task-agent 所用模型能力远弱于 meta-agent 和 feedback-agent]]，导致基线偏弱、结果难以与其他方法直接对比（21:11）。

### 自我改进 Harness 的安全设计：Self-Harness

[[self-harness|Self-Harness]] 让大模型 Agent 通过「提案-评估-接受」循环自主改进自己的 harness，分三阶段：[[self-harness-weakness-mining|弱点挖掘]]需要包含验证层原因、Agent 行为的因果状态、轨迹暴露的抽象机制等丰富信息，因为表面相同的错误背后因果机制可能完全不同（15:08）；[[self-harness-proposal-phase|提案阶段]]输入包括可编辑范围、失败模式、需保留的正确行为、此前修改记录，优先针对反复出现且可通过小范围改动解决的通用错误，并要求候选修改多样化（15:08）；[[self-harness-validation-phase|验证阶段]]要求候选修改在训练集和测试集上都不能出现性能回退才会被接受合并，被拒绝的修改只记录不改动现有系统（15:08）。[[self-harness-terminal-bench-2-result|在 Terminal-Bench-2 上用不同基础模型测试]]，Self-Harness 都能学到针对每个模型弱点定制化的指令，提升通过率（15:08）。安全上，[[self-harness-editable-scope-restriction|可编辑范围必须严格设计]]，若允许改进程序编辑操作系统会打破抽象边界，因此权限控制和安全层必须置于自改进循环之外（15:08），但即便如此 [[reward-hacking-risk|奖励黑客风险依然存在]]（15:08）。

### 尚未解决的核心瓶颈

即便如此，[[harness-vs-intelligence-ceiling|Harness 改进能帮模型更好落地已有能力，但系统能力上限仍取决于基础模型自身智能水平]]（15:08）。文章总结了自动化研究实验（覆盖世界模型、多智能体强化学习、AI 安全三个领域，[[idea-to-paper-generation-experiment|每领域准备四五十篇种子文档]]）中暴露的六个失败模式（21:11）：[[default-solution-bias-failure-mode|默认方案偏见]]（偏向训练数据里过时的库和命令）、[[implementation-drift-failure-mode|实现漂移]]（复杂度高时退而求其次做简单方案）、[[memory-context-degradation-long-horizon|记忆和上下文退化]]（长周期项目丢失关键细节）、[[overoptimism-p-hacking-eureka-effect|过度乐观／p-hacking／eureka 效应]]（实验失败也宣称成功）、[[domain-tacit-knowledge-deficiency|领域隐性知识不足]]（判断不了实现难度和基线重要性）、[[weak-scientific-taste-failure-mode|科学品味弱]]（实验能跑但回答不了真正有价值的问题）。该实验中 [[expert-selected-idea-completion-rate|人类专家最终只挑出四个想法跑完整流程，真正完整生成论文的只有一个]]（21:11）。这也印证了 [[paper-writing-not-scientific-discovery|写论文不等于科学发现]]，尽管 [[ai-scientist-harness-paper-writing|AI Scientist 类工作已证明专家设计的 harness 能协调很大一部分自动研究循环]]，至少在写论文这个形态上已经跑通（21:11）。

更深层的瓶颈包括：[[weak-ambiguous-evaluator-bottleneck|弱且模糊的评估器]]（研究品味、新颖性等难以量化，21:11）、[[negative-results-publication-bias|负面结果的发表偏见]]（人类研究者更愿发表成功案例，21:11）以及 [[context-memory-lifecycle-bottleneck|上下文和记忆生命周期管理]]（agent 越自主，记忆增长越快，21:11）。翁荔认为 [[context-engineering-as-core-intelligence|上下文工程未来应成为智能的核心组成部分]]，而不只是软件系统层（21:11）。此外还有 [[diversity-collapse|多样性坍塌]]问题——进化和强化学习循环倾向利用已知高回报模式，需专门机制防止种群退化，这在开放式研究中尤其重要，因为真正最优路径的初始表现可能并不好（24:11）；[[reward-hacking-self-improvement|奖励黑客]]在不同奖励来源下有不同表现形式（单元测试、裁判模型、基准分数各自的漏洞，24:11），缓解办法是把 [[evaluator-outside-harness-loop|评估器和权限控制放在进化 harness 循环之外]]，配合留出测试、轨迹审计和关键节点人工审核（24:11）；[[failure-preservation-harness-design|好的研究 harness 应方便保存失败尝试]]，从失败中学习是缩小搜索空间的最好方式（24:11）；[[human-data-training-limitation-give-up|由于训练数据大部分是人类创造的]]，模型可能不擅长判断何时该放弃假设、报告负面结果（24:11）；[[sandbox-training-long-term-blindspot|标准沙箱训练难以覆盖可维护性、所有权边界等长期因素]]（24:11），[[short-term-optimization-limitation|编码 agent 目前的优化目标也普遍偏短期]]，难以顾及大型代码库的长期健康（24:11）；[[goodharts-law-objective-drift|训练稳定性和古德哈特定律带来的目标偏移]]仍是尚未解决的挑战（21:11）；[[supervision-scaling-automation-open-problem|如何把人类监督规模化、自动化]]仍是开放问题（24:11），翁荔主张 [[human-role-higher-abstraction|人类应走向更高抽象层级而非被踢出循环]]，在合适的时间、合适层级提供监督（24:11）。最终她将这一切定位为 [[harness-engineering-as-practical-entry-point|Harness 工程是递归自我改进讨论几十年后终于落地的现实切入点]]——不如直接改写权重听起来科幻，但正是这种一步步的工程进展在真正推动方向前进（24:11）。

## 值得记住的细节

- I·J·Good 1965 年提出「超智能机器」，Yudkowsky 2008 年正式命名「递归自我改进」（00:00）。
- 编码 agent 通用工具集：文件系统操作（glob/grep/ls、读写、精确字符串编辑）、Shell（bash/PowerShell）、开发工具（LSP、Git）、外部上下文工具（MCP、技能包、网页搜索）（03:03）。
- ACE 三角色分工：Generator 生成轨迹、Reflector 提炼洞见、Curator 增量更新要点，避免上下文崩塌（06:04）。
- Harness 优化对象升级路径：指令提示词 → 结构化上下文 → 工作流 → Harness 代码 → 优化器代码本身（06:04）。
- Meta-Harness 在 TerminalBench-2 上超过很多人工强基线（09:06）。
- STOP 用能力更弱的 GPT-3.5 / Mixtral 做基础模型时，性能随迭代次数增加反而下降，证明基础模型能力是递归改进的前提（15:08）。
- DGM 以 Claude 3.5 Sonnet 为基础模型，从简单初始配置进化出的 agent 在 SWE-bench Verified 和 Polyglot 上追平/超过人工设计 agent；代码编辑只用 bash + 文件编辑器两个工具（18:11）。
- DGM 父代选择概率与性能成正比、与已产生后代数量成反比（避免过度集中）（18:11）。
- SIA 权重更新用 LoRA + 强化学习，但实验存在混淆因素，task-agent 模型能力远弱于 meta/feedback agent，基线偏弱（18:11、21:11）。
- 自动化研究实验中人类专家最终只选出 4 个想法完整跑流程，真正完整生成论文的只有 1 个（21:11）。
- 六大失败模式：默认方案偏见、实现漂移、记忆/上下文退化、过度乐观（p-hacking/eureka）、领域隐性知识不足、科学品味弱（21:11）。
- Self-Harness 三阶段（弱点挖掘 → 提案 → 验证）要求候选修改在训练集和测试集都不能回退才会被合并（15:08）。
- 进化搜索适用条件：搜索空间大/不规则、难梯度优化、但候选评估容易——Harness 搜索恰好符合（15:08）。

## 这个视频适合谁 / 可以跳过什么

适合对 AI Agent 系统设计、自动化研究工具链（AI Scientist、Meta-Harness、DGM 等）、以及「递归自我改进」话题从哲学思辨走向工程实践感兴趣的技术从业者，尤其是关注编码 Agent 和上下文工程的开发者。如果只想快速了解结论，可以重点看开头的 Harness 定义部分（00:00）和结尾的瓶颈总结（21:11-24:11），中间大段关于 AlphaEvolve、ShinkaEvolve、Promptbreeder、GEPA 等具体进化算法变种的细节（15:08-18:11）如果不打算深入研究进化搜索方法本身，可以选择性跳过。
