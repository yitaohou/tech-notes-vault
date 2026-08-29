---
video_id: z_F0z7wF5XU
url: https://www.youtube.com/watch?v=z_F0z7wF5XU
title: AI自我递归改进先要靠Harness工程 | Lilian Weng最新长文 | 反馈循环 | 三个设计模式 | 核心智能 | ACE | MCE |
  Meta-Harness | STOP
channel: Best Partners TV
published: '2026-07-09'
duration: '26:48'
transcript_origin: subs
tags:
- video
---

# AI自我递归改进先要靠Harness工程 | Lilian Weng最新长文 | 反馈循环 | 三个设计模式 | 核心智能 | ACE | MCE | Meta-Harness | STOP

摘要: [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核-summary|完整摘要]]

## 知识点

- [[ace-curator-incremental-bullet-design]] — 为避免迭代重写过程中出现上下文崩塌和简洁性偏差，ACE的Curator不重写整段提示词，而是输出带标识的结构化要点，通过确定性逻辑合并进上下文日志并定期精简去重。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[ace-generator-reflector-curator-roles]] — ACE系统中，Generator负责参考现有要点生成任务轨迹，Reflector负责从成功和失败的轨迹中提炼洞见，Curator负责用增量条目更新结构化上下文。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[ace-self-managed-memory-limitation]] — ACE已经具备从运行轨迹中学习经验、自我管理记忆的雏形，但其更新规则和整体工作流仍然是人工设计的。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[ads-automated-design-agentic-systems]] — ADAS 先在存档里初始化思维链、自我优化等简单 agent 方案，再让元 agent 参考存档中的现有方案编写新的 agent 代码：先写高层工作流描述，再实现为可执行代码，并经两轮自我优化检查新颖性与正确性，评估合格的新 agent 即加回存档，如此反复迭代。（[12:08](https://youtu.be/z_F0z7wF5XU?t=728)）
- [[aflow-agentic-workflow-search]] — AFlow 从初始工作流模板出发，每轮按分数与探索的混合策略选择一个节点，让大模型根据评估结果修改生成新工作流，执行评估后有提升的工作流加回搜索树，直到分数平稳或用完计算预算。（[12:08](https://youtu.be/z_F0z7wF5XU?t=728)）
- [[agent-definition]] — 早期业界常用的定义是 Agent 等于大模型加记忆加工具加规划加行动；Harness 工程在此基础上新增了工作流设计、评估、权限控制和持久状态管理，重心从写提示词模板转向运行时和软件系统设计。（[00:00](https://youtu.be/z_F0z7wF5XU?t=0)）
- [[agentic-context-engineering-ace]] — ACE不把上下文当成越堆越长的提示词，而是当成一本不断演化的、带标识符和描述的要点式操作手册。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[agentic-workflow-design-as-search-problem]] — 既然 agent 工作流的设计空间很大，就可以把工作流设计本身当成搜索问题，用算法而非人工来寻找更优解，这一思路催生了 ADAS、AFlow 等自动化搜索方法。（[12:08](https://youtu.be/z_F0z7wF5XU?t=728)）
- [[ai-scientist-harness-paper-writing]] — AI Scientist 这类工作已经有力证明，专家设计的 harness 能协调很大一部分自动研究循环，至少在写论文这个形态上已经跑通。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[ai-scientist-system]] — AI Scientist系统搭建了覆盖提出研究想法、写代码跑实验、分析结果、撰写论文到执行同行评审的完整自动研究流水线。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[alphaevolve]] — AlphaEvolve 作为编码 Agent 进化搜索系统，内部维护一个候选程序池，并用参数冻结的大模型生成 diff 补丁来改进程序。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[alphaevolve-meta-prompt-coevolution]] — AlphaEvolve 中元提示词会和指令、上下文一起随大模型的建议共同进化，就像进化解决方案程序一样。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[alphaevolve-prompt-design]] — AlphaEvolve 提示词包含父程序、运行结果、指令，有时还包含元信息，让编码 agent 能访问完整代码仓库，但需改进的区域会用专门标记明确标出。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[autodata-agent]] — AutodataAgent定位为自动的数据科学家，专门生成训练和评估数据，其主Agent管理挑战者、弱求解器、强求解器、验证裁判四个角色，目标是合成难度刚好的任务。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[challenger-solver-verifier-loop]] — 该方法生成的合成数据只用来微调弱模型、不会迭代改进强模型，因此更接近间接的知识蒸馏，自我改进的属性并不强。（[12:08](https://youtu.be/z_F0z7wF5XU?t=728)）
- [[coding-agent-harness-convergence]] — 主流编码agent的通用循环是：先观察整个代码仓库、做规划，接着搜索和读取相关文件，再编辑或打补丁写测试，然后运行检查错误，循环往复直到任务完成，就像人类开发者用 IDE 工作一样。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
- [[coding-agent-toolset]] — 编码agent的通用工具集包括：文件系统操作（glob/grep/ls查找、单文件与批量读取、全量写入、精确字符串替换编辑、批量编辑、结构化补丁）；Shell执行（bash或PowerShell命令）；开发相关工具（语言服务器协议LSP、Git的状态查看/差异对比/提交）；以及外部上下文工具（MCP、技能包、网页搜索与页面抓取）。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
- [[context-engineering-as-core-intelligence]] — 翁荔认为，就像人类能终身维持记忆一样，上下文工程未来应该成为智能的核心组成部分，而不只是停留在软件系统层。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[context-function-file-implementation]] — 在实现层面，一个上下文函数就是专门目录里的一堆文件，既有静态的技能说明文档，也有动态生成的上下文和运行数据。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[context-management-layer]] — 上下文管理层的作用是为大模型构建更结构化、更精简的上下文，同时管理持久状态，用以避免Agent任务周期变长时上下文体量失控。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[context-memory-lifecycle-bottleneck]] — 随着 AI agent 变得越来越自主，记忆会不断增长，一个好用的 harness 需要管理好上下文和记忆，弥补当前长上下文生成的局限，同时最大化长周期任务的成功率。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[darwin-godel-machine]] — 达尔文哥德尔机（DGM）与此前聚焦优化具体解决方案的方法不同，明确把优化目标对准了可编辑的 Harness 代码仓库，让编码 agent 修改自己的 Harness。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[default-solution-bias-failure-mode]] — 实验总结的第一个反复出现的失败模式是模型偏向训练数据里的默认方案，习惯用过时的库、旧的命令、标准格式，假设不是基于实际的仓库或数据集。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[dgm-code-editing-tools]] — DGM 的代码编辑仅依靠 bash 命令和文件编辑器两个基础工具实现，新生成的 agent 需经评估、性能足够好才会加回种群，如此反复迭代直到触发停止条件。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[dgm-experiment-results]] — DGM 实验以 Claude 3.5 Sonnet 作为基础模型，从简单的初始 Harness 配置出发，进化出的 agent 在 SWE-bench Verified 和 Polyglot 基准上能赶上甚至超过手工设计的 agent。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[dgm-fixed-model-harness-evolution]] — DGM 本质是固定模型下的 Harness 进化，不涉及模型权重的更新。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[dgm-limitations]] — DGM 类方法只适合能自动评估、适应度容易量化的场景（如矩阵乘法优化、GPU 内核开发、算法竞赛、数据中心调度），对评估慢、标准模糊、依赖主观判断的领域难以适用，且计算效率与进化有效性仍是待解决问题。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[dgm-parent-selection]] — DGM 选择父 agent 的概率与其性能成正比、与其已产生的后代数量成反比。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[dgm-workflow]] — DGM 从种群中只有一个编码 agent 开始，按性能正比、后代数量反比的概率选择父 agent，令其检查自身基准测试日志并提出对自己 Harness 代码库的改进，生成新版本 agent。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[diversity-collapse]] — 进化和强化学习的循环都倾向于利用已知的高回报模式，需要专门机制防止种群退化成同一种解决方案的不同变种。（[24:11](https://youtu.be/z_F0z7wF5XU?t=1451)）
- [[domain-tacit-knowledge-deficiency]] — 第五个失败模式是领域智能不足，缺少隐性的行业经验，比如判断不了实现难度、实验结果是否合理、哪些基线是重要的。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[evaluator-outside-harness-loop]] — 缓解 reward hacking 的做法是把评估器和权限控制放在进化 harness 的循环外面，配合留出测试、轨迹审计和关键节点人工审核。（[24:11](https://youtu.be/z_F0z7wF5XU?t=1451)）
- [[evolutionary-search]] — 进化搜索特别适合搜索空间很大或形状不规则、难以直接用梯度优化、但评估候选解容易这两类场景，Harness 搜索恰好同时符合这两个特点。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[expert-selected-idea-completion-rate]] — 该实验中人类专家最终只挑出四个想法跑完整流程，其中真正完整生成论文的只有一个。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[failure-preservation-harness-design]] — 一个好的研究 harness 应该让失败的尝试也能被方便地保存下来，从失败中学习才是缩小任务搜索空间的最好方式。（[24:11](https://youtu.be/z_F0z7wF5XU?t=1451)）
- [[file-system-persistent-memory]] — 长周期 agent 运行会产生实验日志、代码差异、论文摘要、错误栈、历史执行轨迹等产物，这些内容长度很快会超过模型训练时的上下文窗口，因此需要用文件系统而非上下文来存储持久状态。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
- [[gepa]] — GEPA 将反思式提示词与进化搜索结合，通过对试错轨迹进行自然语言反思来生成提示词的更新方向。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[goodharts-law-objective-drift]] — 自我改进系统的训练稳定性、以及古德哈特定律带来的目标偏移，是目前尚未得到很好解决的挑战。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[harness-as-code]] — 如果大模型能够直接优化执行 agent 的代码，那它能接触到的设计空间远比只优化手写提示词要大得多。（[12:08](https://youtu.be/z_F0z7wF5XU?t=728)）
- [[harness-as-optimization-target]] — Harness系统本身会成为被优化的目标，人工设计的启发式规则会逐渐减少，通用机制会逐渐增多。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[harness-candidate-directory-structure]] — Meta-Harness生成的每个候选Harness都对应文件系统里的一个目录，包含自己的源代码、评分、运行轨迹和状态更新。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[harness-design-as-search-space]] — Meta-Harness实验结果背后的启示是：一旦Harness设计变成了可执行的搜索空间，强编码Agent就能探索和人类工程师完全一样的设计空间。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[harness-engineering]] — Lilian Weng 认为，连接原始模型与真实应用场景之间的部署系统（harness），其重要性可能不亚于模型本身的原生智能。（[00:00](https://youtu.be/z_F0z7wF5XU?t=0)）
- [[harness-engineering-as-practical-entry-point]] — 递归自我改进这个话题讨论了几十年，现在终于从纯哲学思辨落到具体的工程路径上，Harness 工程就是当下最现实的切入点，虽不如直接改写模型权重听起来科幻，但正是这种一步步的工程进展在真正推动这个方向前进。（[24:11](https://youtu.be/z_F0z7wF5XU?t=1451)）
- [[harness-goal-directed-loop-pattern]] — 与静态提示词模板不同，目标导向循环模式更强调模型在运行时持续分析自己的执行轨迹和失败案例，一步步迭代推进任务。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
- [[harness-improvement-internalization]] — 长期来看，很多Harness的改进可能会被内化到核心模型的行为中，但外部上下文和工具的接口层预计会一直存在。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[harness-meta-methodology-evolution]] — 近期Harness工程会朝着元方法论方向演化，即改进获取答案的机制本身，而不只是改进答案内容。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[harness-optimization-target-escalation]] — 随着模型能力增强，Harness系统中被优化的对象逐步升级：从指令提示词，到结构化上下文，到工作流，到Harness代码，最终到优化器本身的代码。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[harness-vs-intelligence-ceiling]] — Harness 改进能帮助模型更好地落地发挥已有能力，但决定系统能力上限的核心还是基础模型自身的智能水平。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[harness-vs-weight-update-recursive-improvement]] — 此前讨论的 DGM 等方法都停留在 Harness 层面优化模型外的非参数系统，而完整的递归自我改进也可以让模型通过改进训练流水线或测试时持续学习来同时更新自身权重。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[harness-workflow-automation-pattern]] — 工作流自动化是 Harness 反复出现的三个核心设计模式中的第一个，核心是给模型定义一套可以操作、测试、迭代的工作流。（[00:00](https://youtu.be/z_F0z7wF5XU?t=0)）
- [[human-data-training-limitation-give-up]] — 大模型训练数据至少目前大部分是人类创造的，所以模型可能不擅长判断什么时候该放弃一个假设、报告负面结果，甚至承认失败。（[24:11](https://youtu.be/z_F0z7wF5XU?t=1451)）
- [[human-role-higher-abstraction]] — 人类应该往更高的层级走，而不是被踢出循环，即在合适的时间、合适的抽象层级提供监督。（[24:11](https://youtu.be/z_F0z7wF5XU?t=1451)）
- [[hyperagents]] — Hyperagents 在 DGM 基础上进一步引入元 agent，专门负责控制怎么修改现有任务 agent 以及生成新 agent。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[idea-to-paper-generation-experiment]] — 该实验中 agent 可以生成和读取文档作为上下文的一部分，实验覆盖世界模型、多智能体强化学习、AI 安全三个领域，每个领域准备四五十篇高质量种子文档用来启发新想法。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[implementation-drift-failure-mode]] — 第二个失败模式是执行压力下的实现漂移，当实现技术复杂度变高，模型可能会退而求其次做一个更简单的通用方案，而不是真正实现提出的方法。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[karpathy-autoresearch]] — Andrej Karpathy 的 autoresearch 被 Lilian Weng 举例为工作流自动化设计模式的一个很干净的例子。（[00:00](https://youtu.be/z_F0z7wF5XU?t=0)）
- [[lightweight-process-manager]] — 在子agent与后台任务模式中，主agent需要一个轻量的进程管理器，负责启动任务、查看日志、取消失败的运行，最后把结果合并回主线程。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
- [[long-context-context-engineering-interplay]] — 尽管长上下文研究一直在进步，但现阶段长上下文的智能表现和上下文工程往往交织在一起。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[manual-harness-design-era]] — 早期的Harness工作流都是由领域专家手工设计的，直到出现像Meta-Harness这样可以自动搜索优化Harness设计的方法。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[mature-harness-automated-research-loop]] — 成熟的Harness能够支撑起自动研究的闭环，反过来推动模型自我改进。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[mce-framework]] — MCE框架分为两个层级：元层级负责技能的演化，基础层级负责针对给定技能做上下文优化。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[mce-two-level-optimization]] — MCE的优化是双层的：内层在给定技能的前提下于训练数据上搜索最优上下文，外层则在验证集上比较不同技能、挑选性能最好的技能。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[memory-context-degradation-long-horizon]] — 第三个失败模式是记忆和上下文退化，长周期项目会丢失关键细节，除非把日志都写成持久化的产物。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[meta-agent-feedback-agent-task-agent-architecture]] — 在某自我改进系统的实验中，task-agent 所用模型的能力强度远低于 meta-agent 和 feedback-agent，导致整体基线偏弱，结果难以与其他方法直接对比。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[meta-agent-skill-crossover]] — 元级Agent会基于技能数据库中的历史技能进行交叉，生成新的技能，再交给基础级的上下文工程执行，并根据运行反馈优化具体的上下文。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[meta-base-level-shared-tooling]] — MCE的元级和基础级优化都在标准的编码Agent环境里运行，用的是读写、编辑、bash、文件查找这些最基础的工具。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[meta-context-engineering-mce]] — Meta Context Engineering（MCE）把上下文管理的机制本身和上下文里的内容分离开来，是在ACE基础上更进一步的自我改进方向。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[meta-harness]] — Meta-Harness的优化对象是Harness本身，即决定信息该怎么存储、检索、呈现给模型的整套代码，因此得名「用来优化Harness的Harness」。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[meta-harness-outer-loop]] — Meta-Harness的外层循环是：先初始化一批Harness候选，在文件系统中存下每个Harness的代码、分数、运行轨迹；每轮迭代提案者读取历史Harness和对应分数生成新候选，候选通过接口验证后拿去评估，合格的加入池子；迭代结束后输出所有帕累托最优（Pareto optimal）的Harness。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[meta-harness-proposer-agent]] — Meta-Harness中的提案者本身就是一个编码Agent，它用grep、cat等命令读取文件系统中存储的历史执行记录，而不是把所有内容都塞进提示词上下文。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[negative-results-publication-bias]] — 第三个核心瓶颈是负面结果，人类研究者有动力发表成功的结果，所以文献里成功案例多、失败案例少。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[observable-parallel-process-requirement]] — 如果子agent的输出只存在临时的聊天上下文里，很快就会失效且无法追溯；但如果都存成文件、日志、状态记录，模型即使中途被打断也能恢复，还能基于完整执行历史做推理。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
- [[overoptimism-p-hacking-eureka-effect]] — 第四个失败模式是过度乐观，哪怕实验有噪音甚至失败了，模型也会宣称成功，靠数值补丁强行凑结果然后宣布胜利，这也是此前研究里提到的 p-hacking 和 eureka-ing 现象。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[paper-writing-not-scientific-discovery]] — 写论文不等于真正的科学发现，一个系统可以写出看起来很合理的论文，但可能存在伪造引用、实现漂移、实验结果薄弱等问题。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[prompt-engineering-decline-precedent]] — 早年的提示工程提供了先例，随着指令微调和模型推理能力提升，手动提示技巧的重要性下降，但定义目标、约束、上下文和评估的需求从未消失。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[promptbreeder]] — Promptbreeder 通过丰富的变异操作来进化优化任务特定的提示词，其特点是连用来变异提示词的指令本身也会随进化过程一起演化。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[recursive-self-improvement]] — I·J·Good 在 1965 年提出「超智能机器」概念，指能在所有智力活动上超越人类、并能设计出更好机器来改进自己的系统。（[00:00](https://youtu.be/z_F0z7wF5XU?t=0)）
- [[recursive-self-improvement-harness-vs-intelligence-debate]] — 翁荔认为长期来看Harness层与核心智能在自我改进中各自占比难以预判，但近期的自我改进路径大概率不会从模型直接改写权重开始。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[reward-hacking-risk]] — 即便 Self-Harness 已引入权限控制和安全层，奖励黑客（reward hacking）相关的风险依然存在。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[reward-hacking-self-improvement]] — 若奖励来自单元测试，agent 可能过拟合测试；若来自裁判模型，可能学到针对该裁判的奖励黑客技巧；若来自基准分数，则可能利用基准本身的缺陷。（[24:11](https://youtu.be/z_F0z7wF5XU?t=1451)）
- [[sandbox-training-long-term-blindspot]] — 可维护性、所有权边界、迁移成本、向后兼容性、未来的调试负担，这些东西标准沙箱里的训练是很难覆盖到的。（[24:11](https://youtu.be/z_F0z7wF5XU?t=1451)）
- [[scientistone]] — ScientistOne把可验证性作为核心设计约束，要求引用、数值、方法或最终结论等每一个论断都必须能追溯到证据来源，并通过证据链检查来做审计。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[self-harness]] — Self-Harness 让大模型 Agent 通过“提案-评估-接受”的循环自主改进自己的 harness，整个流程分为弱点挖掘、Harness 提案、提案验证三个阶段。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[self-harness-editable-scope-restriction]] — 如果允许 Self-Harness 的改进程序编辑操作系统，系统的抽象边界就会被打破，因此可编辑范围必须严格设计，权限控制和安全层必须置于自改进循环之外。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[self-harness-proposal-phase]] — Harness 提案阶段的输入包括当前 harness 可编辑的范围、失败模式、需要保留的正确行为、以及此前尝试过的修改记录四部分，修改优先针对反复出现且可通过小范围改动解决的通用错误，并要求候选修改尽量多样化、差异化。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[self-harness-terminal-bench-2-result]] — 在 Terminal-Bench-2 基准上分别用不同基础模型测试，Self-Harness 都能学到针对每个模型弱点定制化的 harness 指令，从而提升测试集的通过率。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[self-harness-validation-phase]] — 提案验证阶段要求候选修改在训练集和测试集上都不能出现性能回退才会被接受并合并生成新一代 harness，被拒绝的修改只做记录、不会改动现有系统。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[self-harness-weakness-mining]] — 弱点挖掘阶段的失败记录需要包含验证层原因、相关 Agent 行为的因果状态、轨迹暴露的抽象机制等丰富信息，因为表面相同的错误（如超时或缺少产物）背后的因果机制可能完全不同，只有信息足够丰富才能挖到根因。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[self-taught-optimizer-stop]] — STOP 定义了「元效用（meta-utility）」——优化器在一系列下游任务上的平均效用——并通过递归方式用上一代优化器优化自身，生成下一代优化器。（[12:08](https://youtu.be/z_F0z7wF5XU?t=728)）
- [[shinka-evolve]] — ShinkaEvolve 新增三个组件来提升采样效率：父代采样策略、代码新颖性拒绝采样、元草稿本总结机制。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[shinka-evolve-meta-scratchpad]] — ShinkaEvolve 会在元草稿本里总结此前成功的变异模式，用以指导后续新变异的生成方向。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[shinka-evolve-novelty-rejection]] — ShinkaEvolve 使用基于嵌入相似度的代码新颖性拒绝采样，丢弃与已有候选过于相似的重复方案。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[shinka-evolve-parent-sampling]] — ShinkaEvolve 的父代采样策略会同时平衡个体的性能排名与其已产生的后代数量。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[short-term-optimization-limitation]] — 编码 agent 已经能提升日常软件开发效率，但很多优化目标还是太短期，只能完成手头任务，难以顾及几百上千人共同维护的代码库的长期健康。（[24:11](https://youtu.be/z_F0z7wF5XU?t=1451)）
- [[sia-agent-roles]] — SIA 中元 agent 负责提出初始 Harness，任务特定 agent 负责执行具体任务，反馈 agent 根据最近的运行轨迹决定下一步是更新 Harness 还是更新模型权重。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[sia-confounding-factors]] — 翁荔提到 SIA 这项工作的实验设计存在一些混淆因素，需要谨慎解读其结果。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[sia-lora-weight-update]] — SIA 的权重更新采用 LoRA 方式，通过强化学习来完成。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[sia-self-improving-agent]] — SIA 是把 Harness 改进和模型参数更新放在同一个优化循环里的早期尝试。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[skill-as-context-function]] — 在MCE的定义里，一个技能对应一个上下文函数，包含静态组件（提示词、知识库、代码库等固定内容）和动态算子（搜索、选择、筛选、格式化等操作）两部分。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[skill-database]] — MCE系统维护一个技能数据库，记录所有历史生成过的技能、其对应的上下文函数以及评估指标，供元级Agent参考使用。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[stop-self-improving-optimizer]] — STOP 框架下，若把基础模型换成能力更弱的 GPT-3.5 或 Mixtral，随迭代次数增加性能反而下降，说明光有递归改进结构不足以带来提升，基础模型必须具备足够强的能力才能真正改进机制本身。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- [[stronger-model-prevents-harness-overengineering]] — 更强的模型能够避免Harness走向过度工程化，从而让系统保持可持续性。（[06:04](https://youtu.be/z_F0z7wF5XU?t=364)）
- [[subagent-background-task-pattern]] — 当主 agent 需要同时验证多个假设、并行跑实验，或把孤立的子任务委派出去以避免污染主上下文时，子agent与后台任务模式非常有用。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
- [[supervision-scaling-automation-open-problem]] — 怎么把监督规模化、自动化，还是一个开放的研究问题。（[24:11](https://youtu.be/z_F0z7wF5XU?t=1451)）
- [[terminalbench-2]] — 在TerminalBench-2基准上，Meta-Harness优化出来的方案表现超过了很多人工编写的强基线。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
- [[theta-evolve]] — ThetaEvolve 把进化搜索和强化学习、上下文学习结合起来，是 AlphaEvolve 的后续变种之一。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
- [[weak-ambiguous-evaluator-bottleneck]] — 现在的自我改进循环在有可衡量客观指标的任务上效果最好，逻辑和强化学习一样；但研究品味、新颖性、长期科学价值这些东西都很难量化，是弱且模糊评估器带来的瓶颈。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
- [[weak-scientific-taste-failure-mode]] — 第六个失败模式是科学品味弱，实验虽然能跑，但回答不了真正有价值的问题。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
