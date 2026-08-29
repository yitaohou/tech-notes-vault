---
video_id: Mi5wOpAgixw
title: Multi-agent Systems Explained in 17 Minutes
source: '[[2026-02-22-multi-agent-systems-explained-in-17-minutes]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: 79aeda9d542353b43f3e7e98061d7d0738d0f83c90f494688302cbe81180e567
  schema_version: 1
  model: sonnet
  generated_at: '2026-08-26T19:28:43+00:00'
---

## 一句话总结

2025 年是 [[single-agent-2025-multi-agent-2026-prediction|single agent 系统走向成熟的一年]]，而 [[multi-agent-systems]] 并非 [[multi-agent-not-pareto-improvement|单代理系统的帕累托改进]]，是否使用多代理取决于任务是否可分解、单代理成功率高低以及成本优先级,而当前最大的瓶颈是 [[multi-agent-harness-best-practices-gap|尚无公认的 harness 最佳实践]]。

## 核心内容

### 为什么需要 multi-agent:test-time compute 与 context rot 的矛盾

[[test-time-compute-scaling|test-time compute scaling]] 的核心原则是 agent 思考越久、执行的 tool call 和与真实世界的交互越多，任务表现就越好（00:00）。但 [[chromadb-context-rot-study|ChromaDB 的研究]]发现，即使是百万 token 级别的大上下文窗口，随着窗口填充度增加，各前沿模型在简单的单词重复任务上表现依然明显下降，这就是 [[context-rot|context rot]] 现象（00:00）。这形成了一个核心张力：[[test-time-compute-context-tension|更多 token 有利于表现，但上下文填得越满又会因 context rot 拖累表现]]（00:00）。[[multi-agent-systems]] 正是通过让多个 agent 分担工作，在扩大整体算力用量的同时避免单个 agent 上下文塞爆，例如同时启动数十个 [[deep-research-agent|research agent]] 分别独立调研不同关键词，再汇总发现（00:00），这也体现了 [[parallel-agent-execution|并行执行]]和 [[agent-specialization|专业化分工]]的优势。2025 年被称为 AI agent 元年，[[deep-research-agent]] 和 [[coding-agent]] 的兴起是这一趋势的重要体现（00:00）。

### 该不该用 multi-agent:任务类型与成本是关键判据

[[single-agent-first-principle|构建 agent 系统应先从单代理开始]]评估能力，只有满足特定标准后才转向多代理（06:02）。核心判据是[[task-decomposability-determines-agent-architecture|任务是否可分解]]:如果任务是顺序性的——执行、获取信息、据此更新计划、再执行下一步——单代理系统效果更好（03:02）。例如先查阅最新文档、再写 PRD/计划、最后才能构建应用，三步必须严格顺序完成、无法并行,这就是 [[sequential-task-single-agent-advantage|顺序任务适合单代理]]的典型例子（03:20）。相反，若任务可拆解为并行子任务（如同时深入研究 Chroma、Cohere、LlamaIndex 等不同库再汇总综合），[[decomposable-task-multi-agent-advantage|多代理系统更有优势]]（03:35, 04:05）。

但扩展到多代理会引入 [[multi-agent-coordination-cost|agent 间协调的额外计算成本]]（04:40），且这种成本是[[multi-agent-compute-cost-superlinear|超线性的]]——5 个 agent 组成的系统成本会超过单 agent 的 5 倍，因为除了各自消耗算力外还需额外算力用于相互沟通协调（06:02）。[[google-research-45-percent-threshold|Google Research 的论文]]给出了一个量化阈值：若单代理系统成功率超过 45%，不建议用多代理，因为性能提升不足以抵消协调成本；若成功率低于 45%（失败率较高），多代理才可能有帮助（04:45, 05:05）。此外，如果[[cost-priority-single-agent-choice|控制计算成本是最重要的因素]]，单代理是更合适的选择（05:20）。

### 四种 multi-agent 架构:独立、去中心化、集中、混合

[[google-multi-agent-architecture-paper|Google 的论文]]将 multi-agent 系统分为[[independent-multi-agent-architecture|独立式]]、[[decentralized-multi-agent-architecture|去中心化式]]、[[centralized-agent-architecture|中心化式]]和[[hybrid-agent-architecture|混合式]]四类（06:02）。

**独立式**是把同一请求同时发给多个 agent 实例（如 5 个或 10 个），各自独立尝试、互不通信，最后通过 [[voting-aggregation-mechanism|投票或直接择优]]汇总结果（06:02）。优点是实现简单、无需协调机制；缺点是本质上只是同一 agent 多跑几次，通常只带来边际收益提升,而且由于无法相互纠错，[[independent-multi-agent-error-rate|Google 研究发现其错误数量是单代理系统的 17 倍]]，可能并不适合大多数场景（06:02）。适用场景是需求模糊时让多个实例各出方案、择优选用（06:02）。

**去中心化架构**没有层级，所有 agent 地位平等，外部围绕它们搭建一层 [[agent-harness|harness]] 来协调（09:02）。优点是设计简单，只需一组相同的 agent 副本加一层 harness；在大范围探索型任务上表现最佳，是同类架构中 benchmark 表现最好的（09:02）。缺点是协调成本最大：由于每个 agent 都能与所有其他 agent 通信且没有主导者，一个发现要传播给所有人就必须逐一通信或依赖共享上下文，使 harness 设计复杂且需针对任务定制（09:02）。[[decentralized-swarm-architecture|swarm 架构]]比较适合非结构化的探索性研究任务（12:04），15:06 处进一步比喻为"一群 agent 共同围攻同一问题，没有统一领导者调度"。

**中心化架构**由一个 lead agent（orchestrator）负责把任务分派给一组 worker agent，而非让多个 agent 以 swarm 形式自由协作（12:04）。其错误放大程度最低：若某个 sub-agent 出错，错误只会传回 lead agent 由其核实校正，不会立即扩散给其他 sub-agent（12:04）。根据 [[error-amplification-multi-agent|Google 论文]]，在所测试的多种架构中，中心化架构的错误放大程度最低（12:04）。缺点是系统复杂度较高，设计其协调框架本身就是一项非平凡的工作（12:04）。适合目标单一、需要保持连贯性的任务（15:06）。

**混合架构**允许 sub-agent 之间彼此直接通信，不必像中心化架构那样只能经 lead agent 中转（12:04），兼具中心化的纠错能力和去中心化的灵活性，无需像传话游戏一样层层转发（12:04）。但它是几种架构中最复杂的一种，因 teammate 间可直接通信而带来更高的 [[coordination-tax-multi-agent|coordination tax]]，增加计算成本并占用每个 teammate 上下文窗口的 token（12:04）。是介于两种极端架构之间的折中方案（15:06）。[[claude-code-agent-teams|Claude Code 新发布的 agent teams 功能]]即采用混合架构，由 main agent 生成各 sub-agent 并分配任务，teammate 之间共享一个任务列表、可自行认领任务并相互沟通，同时由 main（lead）agent 监督整体进度（12:04）。

Anthropic 自己的[[anthropic-multi-agent-research-system|多智能体研究系统]]也采用中心化式设计：lead agent 拥有一组工具并将任务委派给专门的 sub-agent，包括一个 citations sub-agent 和多个可独立调查特定主题的 search agent，并有一个 running memory 供 lead agent 写入信息，作为整个系统的共享记忆载体（12:04）。

### 案例研究:16 个 agent 两周构建 C compiler

[[single-agent-scale-limitation|单个 agent 很擅长在现有代码库中构建具体功能]]，但像 C compiler 这样的大型单体项目，单个 agent 本身无法胜任（09:02）。[[anthropic-c-compiler-case-study|Anthropic 的案例研究]]中，16 个 agent 协同工作两周构建了这个 C compiler，最终产出约 10 万行 Rust 代码，在相关 benchmark 上达到 99% 准确率，并成功运行了 Doom 游戏（也是一种基准测试），API 调用成本约 2 万美元（09:02）。这里用到的 [[agent-harness|harness]] 可以是一组测试来确认任务完成，也可以是一个任务列表供各 agent 认领并勾选完成（09:02）。

这引出了一个 [[multi-agent-vs-human-cost-quality-tradeoff|质量与速度/成本的权衡]]：想要更快更便宜可以牺牲质量，想要最高质量则需要人类耗费更长时间并支付高于 API 调用的费用。若改由人类开发者构建同一个 C compiler，可能需要数月而非两周，成本可能高达约 10 万美元而非 2 万美元，但最终质量很可能高于多智能体系统的产出（09:02）。

### 现状与展望:没有最优架构，剩下的是工程问题

[[no-optimal-multi-agent-architecture|多智能体系统目前最显著的局限之一是不存在单一最优架构]]，最合适的选择高度依赖具体 use case 和任务类型（12:04）。因此值得通过 [[multi-agent-architecture-experimentation|实验尝试不同架构]]（集中式、去中心化、混合式），找出最适合自己场景的方案（15:06）。作者认为现在模型能力已经足以支撑构建 multi-agent 系统，剩下的主要是[[multi-agent-becomes-engineering-problem|工程问题]]——即针对具体任务构建有效 harness 的挑战（15:06），而[[multi-agent-harness-best-practices-gap|目前还没有公认的最佳实践和标准]]，从业者需要大量试错（15:06）。同时，[[multi-agent-heuristics-obsolescence|当前这套针对现有一代模型总结的设计启发式规则]]，也可能随着模型变得更聪明而过时（15:06）。作者的预测是：[[single-agent-2025-multi-agent-2026-prediction|2025 年是单代理系统成熟的一年，2026 年将是多代理系统成熟的一年]]（15:06）。

## 值得记住的细节

- [00:00] context rot：ChromaDB 研究显示，即便上下文窗口有百万 token 级别，随填充度增加各前沿模型在简单单词重复任务上表现明显下降。
- [04:45] Google Research 论文给出的关键阈值：单代理成功率 **>45%** → 不建议上多代理；**<45%** → 多代理可能有帮助。
- [06:02] 独立式架构：错误数量是单代理系统的 **17 倍**（因无法相互纠错）。
- [06:02] 多代理算力成本是超线性的：5 个 agent 的系统成本会**超过**单代理的 5 倍。
- [09:02] Anthropic C compiler 案例：**16 个 agent、2 周、约 10 万行 Rust 代码、99% 准确率、成功跑通 Doom、API 成本约 2 万美元**；对比人类开发可能需要数月、约 10 万美元成本，但质量可能更高。
- [12:04] Claude Code 的 agent teams 功能采用 hybrid architecture，teammate 共享任务列表、可互相通信，main agent 监督进度。
- [12:04] 根据 Google 论文，在测试的架构中 centralized architecture 的错误放大程度最低；hybrid architecture 因 sub-agent 间可直接通信而 coordination tax 最高、最复杂。
- [15:06] 三种架构的简明类比：centralized = 一个 lead 分派任务给 workers（目标单一、连贯性要求高）；decentralized = swarm 围攻同一问题，无领导者（探索型任务最佳）；hybrid = 两者折中。

## 这个视频适合谁 / 可以跳过什么

适合：正在评估是否要从 single agent 系统升级到 multi-agent 系统的开发者/架构师，想理解 independent / decentralized / centralized / hybrid 四种架构取舍的人，以及关注 2025→2026 agent 技术趋势判断的从业者。

可以跳过：如果你的任务本质上是顺序性的（[[sequential-task-single-agent-advantage]]），或者当前单代理成功率已经较高（>45%）且成本敏感，视频反复强调此时不必折腾 multi-agent，可直接跳到 15:06 处的总结结论即可，无需细究中间四种架构的具体案例（09:02–12:04 的 C compiler 与 Claude Code 细节可选看）。
