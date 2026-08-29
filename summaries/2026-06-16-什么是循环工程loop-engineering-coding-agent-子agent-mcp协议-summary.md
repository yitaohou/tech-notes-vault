---
video_id: KgiwIEBeOHw
title: 什么是循环工程Loop Engineering | Coding Agent | 子Agent | MCP协议 | 提示词工程 | AI开发效率 |
  软件研发 | Addy Osmani
source: '[[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: 8a694a5e5d1d8a4475dc7f2b25c219eab811d4243df57b40ec00119c0d932755
  schema_version: 1
  model: sonnet
  generated_at: '2026-08-26T19:55:47+00:00'
---

## 一句话总结

循环工程（[[loop-engineering]]）主张程序员的核心工作正从"给 Coding Agent 写提示词"转向"设计一套能自主运转、直到目标达成才停止的循环系统"，而 Claude Code 与 Codex 已经各自内置了构成这套循环的五大模块，真正的瓶颈不再是工具能力，而是人的审核带宽与循环设计者的判断力（18:06）。

## 核心内容

### 从手动提示到循环工程的转向

Claude Code 负责人 [[boris-cherny]] 表示自己已经不再手动提示 Claude，而是让很多循环在后台运行、自动决定下一步做什么，他的核心工作变成了编写这些循环（00:00）。这与 Andrej Karpathy 的 [[karpathy-autoresearch]] 思路一致：把人从循环中抽离，让系统自主运行、最大化 token 吞吐量，人不再是流程瓶颈（00:00）。OpenClaw 开发者 [[peter-steinberger]] 也持相同立场：不该再手动提示 Agent，而应设计让 Agent 自动运行的循环（00:00）。[[loop-engineering-recursive-goal]] 的核心是人只定义最终目标，AI 在循环里反复迭代直到达成，无需人工逐轮触发（00:00）。

这一理念之上还有历史脉络：循环工程之前已有 [[harness-engineering]]（为单个 Agent 搭运行环境）和 [[factory-model]]（整套软件构建系统）两个概念，[[loop-engineering]] 位于 harness engineering 之上一层，是跑在计时器上、能自主生成子 Agent 并自我驱动的运行环境（03:01）。大约一年前想跑一个自动循环还得自己写一堆难以复用的 bash 脚本（[[loop-engineering-diy-history]]，03:01），如今 [[codex]] 和 Claude Code 已把这些能力产品化，不必再从零搭建。

### 五大模块：自动化、工作树、Skill、目标循环、连接器

一套完整循环由 [[loop-system-five-modules]] 五个核心模块加一个独立记忆载体构成，Claude Code 和 Codex 已完整具备（[[loop-engineering-five-building-blocks]]，00:00）：

**自动化模块**（[[automation-module]]）是循环的"心跳"，负责主动发掘任务，其余模块处理被发掘出的任务（[[loop-automation-module-role]]，03:01）。Codex 的[[codex-automation-tab|自动化标签页]]可设定项目、提示词、频率及运行环境；发现问题进[[codex-automation-triage-inbox|分类收件箱]]，无问题则自动归档（03:01）。Claude Code 则用 [[claude-code-loop-command|/loop 指令]]与[[claude-code-scheduling-hooks|调度、钩子]]实现同等能力，[[claude-code-hooks-lifecycle]]可在生命周期节点触发 shell 命令，还能调用 [[automation-skill-invocation|Skill 名称]]而非粘贴一堆指令。若要脱离本机持续运行，可接入 [[github-actions-loop-persistence|GitHub Actions]]（03:01）。OpenAI 内部就用自动化处理 issue 分类、CI 失败汇总、提交简报、bug 排查等重复工作（[[openai-internal-automation-use-cases]]，03:01）。不同工具实现路径不同，但[[loop-automation-core-logic|核心逻辑]]一致：定义自主任务、设定节奏、主动反馈（03:01），这也印证了[[coding-agent-harness-convergence|不同 Coding Agent 底层架构已趋同]]，选哪款工具不再关键，重要的是设计通用循环逻辑。

**工作树模块**（[[git-worktree-multi-agent-isolation]]）解决多 Agent 并行时的文件冲突：工作树共享同一仓库历史但拥有独立工作目录和分支，从物理层面隔离不同 Agent 的修改。Claude Code 通过 `--worktree` 参数开启隔离会话并自动清理，Codex 则直接内置支持，多线程可同时访问同一仓库（06:03）。但这只解决了机械层面的冲突，真正的瓶颈仍是人：一个人一天能认真审核多少代码产出才是并行上限，这被称为[[agent-parallelism-human-review-bottleneck|编排税]]（06:03）。

**Skill 模块**（[[coding-agent-skills-context-reuse]]）解决每次新会话都要重新解释项目规范的问题：Claude Code 与 Codex 采用相同格式——一个文件夹存放说明文档、指令、元数据及可选脚本资源，可在 Codex 中用符号或指令主动调用（06:03）。Skill 的价值在于避免 [[intent-debt|intent debt]] 的重复消耗，让知识积累产生复利（09:03）；描述文字应简洁准确（[[claude-skills]]，09:03）。若要跨仓库共享或打包多个 Skill，可封装为 [[plugins-content-distribution|Plugin]]，一次安装即可复用整套配置（09:03）。

**目标导向循环**（[[goal-directed-persistent-loop]]）以 `/goal` 指令为代表，不同于按固定节奏运行的 `/loop`，它持续运行直到用自然语言描述的可验证条件达成，例如"认证模块测试全通过且格式检查无误"，Codex 也提供同名功能并支持暂停恢复（06:03）。关键设计是 [[goal-verifier-separate-agent|验证与生成分离]]：判断目标是否完成的是独立的小模型，而非写代码的 Agent 本身（06:03，13:10 对应 [[goal-completion-separate-model-check]]）。

**连接器模块**（[[mcp-connectors]]）让循环能读取需求跟踪器、查询数据库、发送即时消息，而不局限于本地文件系统；由于 Codex 和 Claude Code 都支持 MCP 协议，连接器可跨工具复用（09:03）。这决定了 [[agent-vs-full-loop-distinction|普通 Agent 与完整循环的区别]]：普通 Agent 只能给建议，完整循环能自己创建合并请求、关联工单、CI 通过后自动通知相关人员（09:03）。

### 子 Agent 分工与验证责任

[[sub-agent-code-review-separation]] 指出，让写代码的模型自评往往判断过宽、难以发现自身逻辑漏洞，需要用不同指令甚至不同模型的第二个 Agent 来评审（09:03）。Codex 中子 Agent 仅在用户主动要求时生成，可并行运行后合并结果；子 Agent 可在配置目录中定义名称、描述和指令（09:03）。Claude Code 支持组建 [[claude-code-agent-teams|Agent 团队]]，让任务在不同角色间流转（12:20）。可按角色差异化配置模型与权限（[[role-based-model-permission-config]]）：安全审查用强模型、高推理强度；探索型 Agent 用轻量模型且仅开只读权限（12:04）。最常见的分工模式是 [[explorer-implementer-verifier-agent-pattern|探索-实现-验证三角]]，无论用哪款工具都一致（12:40）。验证环节尤为重要，因为循环常在无人盯着的情况下运行，只有信得过的验证才能放心自动化（[[unattended-loop-trusted-verification]]，12:50）。但子 Agent 会消耗更多 token（每个 Agent 独立调用模型和工具），不宜滥用，只在需要二次把关时开启（[[multi-agent-coordination-cost]]，13:00）。

### 持久记忆与完整案例

大模型本质上没有跨会话记忆（[[ai-context-amnesia-session]]，13:35），因此循环必须依赖 [[file-system-persistent-memory|外部持久化记忆]]——一个 Markdown 文件或项目看板即可，代码仓库和状态文件不会遗忘任务进度（13:25-13:45）。视频给出一个完整案例（[[automated-triage-skill-workflow]]）：每天早上自动化任务调用分类 Skill 读取前一天的 CI 失败、未解决 issue、最近提交，写入 Markdown（14:00）；对每个值得处理的问题创建[[isolated-worktree-per-task|隔离工作树]]并派子 Agent 起草修复（14:20）；第二个子 Agent 对照规范和测试审查修复方案（14:30）；通过后连接器自动创建合并请求、更新工单（[[loop-connector-automation]]，14:40）；处理不了的问题进入[[loop-human-escalation-inbox|人工分类收件箱]]（14:50）；[[loop-state-file-continuity|状态文件]]记录已尝试方案和验证结果，让次日任务接续推进（15:00）。

### 风险与边界：认知投降与理解债

视频最后强调循环工程的核心风险。[[cognitive-surrender|认知投降]]：循环能自主运行后，人容易不再主动判断、直接接受结果，这种最舒服的状态恰恰最危险（15:04）。[[comprehension-debt|理解债]]：循环产出代码越快，开发者未亲手写过的代码越多，代码库与真正理解之间的差距就越大，唯一解法是持续认真阅读循环生成的代码（15:04）。[[generator-verifier-agent-separation]] 虽让"完成"判断更可信，但"完成"本身仍只是声明而非严格验证（15:04）。[[unattended-loop-verification-responsibility]] 点明：无人值守的循环也是无人值守犯错的循环，开发者依然要对亲自确认过的代码负责，这一点循环本身不会改变（15:04）。视频最终结论呼应 [[boris-cherny]]：AI 没有让编程变简单，而是把杠杆点从"写好提示词"转移到了"设计好一套持续运行的系统"（18:06）。

## 值得记住的细节

- Claude Code 用 `--worktree` 参数开启独立代码副本会话，任务结束自动清理工作目录（06:03）
- `/loop` 按固定节奏重复运行，`/goal` 持续运行直到自然语言描述的可验证条件达成，两者用途不同（06:03）
- `/goal` 示例停止条件："认证模块所有测试全部通过，并且代码格式检查没有问题"（06:03）
- Skill 文件结构：一个文件夹 + 说明文档（含指令、元数据）+ 可选脚本/参考资料，Codex 与 Claude Code 格式通用（06:03）
- 想让 Claude Code 自动化流程脱离本机持续运行，可推送到 GitHub Actions（03:01）
- OpenAI 内部自动化用例：issue 每日分类、CI 失败汇总、提交简报、上周新 bug 排查（03:01）
- 子 Agent 会显著增加 token 消耗（每个 Agent 独立完成模型调用和工具使用），仅在需要二次把关时值得开启（13:00）
- 角色化模型配置建议：安全审查 Agent 用强模型+高推理强度；探索型 Agent 用轻量模型+只读权限（12:04）
- 循环记忆载体可以就是一个 Markdown 文件或项目看板，不需要复杂系统（13:25）
- 编排税的实际上限不是工具并发数，而是一个人一天能认真审核多少份代码产出（06:03）

## 这个视频适合谁 / 可以跳过什么

适合已经在用 Claude Code 或 Codex、并想从"手动提示"升级到"自动化循环/自动化任务"的开发者，尤其关心多 Agent 协作、Skill 复用、CI/issue 自动分诊场景的人。如果只关心某一款工具的具体操作命令，可以跳过前段关于 loop engineering 概念起源与行业人物观点的部分（00:00），直接看 03:01 起的五模块拆解和 14:00 的完整案例；对认知投降、理解债等风险不感兴趣、只想学配置的观众，可以跳过 15:04 之后的反思部分，但这部分是视频作者认为最重要的取舍判断，建议不要完全略过。
