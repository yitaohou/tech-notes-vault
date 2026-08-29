---
video_id: KgiwIEBeOHw
url: https://www.youtube.com/watch?v=KgiwIEBeOHw
title: 什么是循环工程Loop Engineering | Coding Agent | 子Agent | MCP协议 | 提示词工程 | AI开发效率 |
  软件研发 | Addy Osmani
channel: Best Partners TV
published: '2026-06-16'
duration: '18:32'
transcript_origin: subs
tags:
- video
---

# 什么是循环工程Loop Engineering | Coding Agent | 子Agent | MCP协议 | 提示词工程 | AI开发效率 | 软件研发 | Addy Osmani

摘要: [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议-summary|完整摘要]]

## 知识点

- [[agent-parallelism-human-review-bottleneck]] — 工作树解决的只是机械层面的文件冲突，整个流程的瓶颈依然是人本身：一个人一天能认真审核多少份代码产出，才是实际能并行运行多少Agent的上限，而不是工具能同时跑多少线程，这被称为编排税。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- [[agent-vs-full-loop-distinction]] — 普通的 Agent 只能告诉用户这里有个修复方案，而完整的循环可以自己创建合并请求、关联对应的需求工单，等持续集成通过之后自动在沟通频道里通知相关人员，因此连接器让循环能真正融入现有工作环境而不只是停留在给出建议的层面。（[09:03](https://youtu.be/KgiwIEBeOHw?t=543)）
- [[ai-context-amnesia-session]] — 大模型有一个本质特点：每次运行之间不会记住之前的内容，所以记忆不能只存在于对话上下文里，必须落到磁盘文件等持久化存储上。（[13:35](https://youtu.be/KgiwIEBeOHw?t=815)）
- [[automated-triage-skill-workflow]] — 一个典型场景是：每天早上一个自动化任务在代码仓库上运行，调用分类Skill读取前一天的持续集成失败记录、未解决issue、最近的代码提交，把发现的问题整理好写入Markdown文件或项目看板。（[14:00](https://youtu.be/KgiwIEBeOHw?t=840)）
- [[automation-module]] — 自动化模块是整个循环的心跳，正是它让循环成为真正持续运转的循环，而不是一次性手动运行的任务。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[automation-skill-invocation]] — 自动化任务可以直接调用对应的 Skill 名称，不用把一大堆指令都粘贴到定时任务里，这样后续维护起来也方便很多。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[boris-cherny]] — Claude Code负责人Boris Cherny表示，自己现在已经不手动提示Claude，而是有很多循环在后台运行，负责提示Claude、判断下一步该做什么，他自己的核心工作就是编写这些循环。（[00:00](https://youtu.be/KgiwIEBeOHw?t=0)）
- [[claude-code-agent-teams]] — Claude Code支持在配置目录里定义子Agent，还可以组建Agent团队，让任务在不同角色的Agent之间流转。（[12:20](https://youtu.be/KgiwIEBeOHw?t=740)）
- [[claude-code-hooks-lifecycle]] — Claude Code 的钩子功能可以在 Agent 生命周期的特定节点触发 shell 命令，用于实现更细粒度的自动化控制。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[claude-code-loop-command]] — 用 /loop 指令可以让一个提示词或命令在 Claude Code 中按照固定间隔重复运行，也可以设置定时任务按自定义周期执行。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[claude-code-scheduling-hooks]] — Claude Code 用调度和钩子两种方式来实现与 Codex 自动化标签页相同的能力。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[claude-skills]] — Skill 的描述文字应力求简洁明确、匹配准确，而非追求花哨表达，因为系统会依据任务描述与 Skill 描述的匹配程度自动触发对应的 Skill，这一逻辑在 Claude Code 中同样适用。（[09:03](https://youtu.be/KgiwIEBeOHw?t=543)）
- [[codex]] — Codex 已将循环工程的核心能力（如自动化任务）直接内置到产品中，无需开发者自行从零搭建。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[codex-automation-tab]] — 在 Codex 的自动化标签页里，用户可以创建任务并选择对应项目、要运行的提示词、执行频率，还能选择在本地代码副本上运行还是在后台工作树里运行。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[codex-automation-triage-inbox]] — Codex 自动化任务每次运行后，如果发现需要处理的问题，结果会进入分类收件箱；如果什么问题都没发现，这次运行就会自动归档，不会产生冗余信息。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[coding-agent-harness-convergence]] — Claude Code 与 Codex 都各自实现了功能几乎相同的/goal 能力，体现出整个编码Agent行业发展方向的高度一致性。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- [[coding-agent-skills-context-reuse]] — Skills 模块用于解决每次开启新会话都要重新向Agent解释一遍项目结构、规范、构建方式的问题。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- [[cognitive-surrender]] — 当循环可以自己运行时，人很容易不再主动思考和判断，直接接受循环给出的所有结果，这种最舒服的状态往往也是最危险的、最容易被忽略的状态，即认知投降。（[15:04](https://youtu.be/KgiwIEBeOHw?t=904)）
- [[comprehension-debt]] — 循环产出代码的速度越快，开发者没有亲手写过的代码就会积累得越多，实际存在的代码与真正理解的内容之间的差距就会越来越大，即理解债。（[15:04](https://youtu.be/KgiwIEBeOHw?t=904)）
- [[explorer-implementer-verifier-agent-pattern]] — 无论用哪款工具，最常见的分工模式都是一致的：一个Agent负责探索需求，一个负责实现代码，还有一个负责对照需求规格做验证。（[12:40](https://youtu.be/KgiwIEBeOHw?t=760)）
- [[factory-model]] — 在循环工程概念出现之前，行业里已有 Agent Harness Engineering（为单个 Agent 搭建运行环境框架）和工厂模型（一整套构建软件的系统）两个相关概念。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[file-system-persistent-memory]] — 循环的记忆系统可以是一个普通的Markdown文件，也可以是一个项目看板，任何能存在于单次对话之外、用来记录已完成事项和待办事项的载体都可以。（[13:25](https://youtu.be/KgiwIEBeOHw?t=805)）
- [[generator-verifier-agent-separation]] — 把生成代码的 Agent 和验证的子 Agent 分开，是为了让循环给出的完成结论更有参考性，但「完成」本身仍只是一个声明，而不是经过严格验证的结论。（[15:04](https://youtu.be/KgiwIEBeOHw?t=904)）
- [[git-worktree-multi-agent-isolation]] — 工作树（Worktrees）模块用于解决多Agent并行运行时的文件冲突问题：同时运行多个Agent很容易出现多个Agent修改同一文件、最终代码冲突导致任务失败的情况。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- [[github-actions-loop-persistence]] — 如果希望任务在关掉电脑之后依然继续运行，可以把整套 Claude Code 自动化流程推送到 GitHub Actions 上执行。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[goal-completion-separate-model-check]] — /goal 指令底层用的也是生成与校验分离的逻辑：判断循环有没有完成的是一个全新的模型，而不是执行任务的那个模型。（[13:10](https://youtu.be/KgiwIEBeOHw?t=790)）
- [[goal-directed-persistent-loop]] — /goal 指令不同于按固定节奏重复运行的/loop，它会持续运行，直到用户设定的条件真正达成为止，无需人工盯着进程。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- [[goal-verifier-separate-agent]] — 在/goal 模式下，每轮执行结束后由一个独立的小模型检查目标是否完成，写代码的Agent与判断任务是否完成的Agent是两个不同的Agent。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- [[harness-engineering]] — Agent Harness Engineering 指为单个 Agent 搭建运行环境框架的工程实践，位于循环工程之下的一层。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[intent-debt]] — Skill 通过把项目的规则、约定、构建步骤甚至过往踩过的坑正式记录下来，使 Agent 每次运行都能读取这些知识，从而避免 intent debt 的重复消耗，并让知识积累产生复利效应。（[09:03](https://youtu.be/KgiwIEBeOHw?t=543)）
- [[isolated-worktree-per-task]] — 对于每一个值得处理的问题，循环都会创建一个隔离的工作树，派出一个子Agent去起草修复方案。（[14:20](https://youtu.be/KgiwIEBeOHw?t=860)）
- [[karpathy-autoresearch]] — Andrej Karpathy提出的AutoResearch项目核心思路是把人从循环中抽离出来，让系统自主运行并尽可能提升token吞吐量，使人不再成为整个流程的瓶颈。（[00:00](https://youtu.be/KgiwIEBeOHw?t=0)）
- [[loop-automation-core-logic]] — 不同 Coding Agent 工具实现自动化的路径虽然不同，但核心逻辑完全相同：定义一个自主运行的任务，设定它的运行节奏，产生结果后会主动反馈，用户不需要主动去四处检查进度。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[loop-automation-module-role]] — 循环系统中的自动化模块负责主动把潜在的工作任务发掘出来，而循环里剩下的模块则用于处理这些被发掘出的任务。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- [[loop-connector-automation]] — 修复方案通过审查后，连接器会让循环自动创建合并请求，并更新对应的需求工单。（[14:40](https://youtu.be/KgiwIEBeOHw?t=880)）
- [[loop-engineering]] — 循环工程的核心理念是：程序员未来的核心工作可能不再是直接给Coding Agent写提示词，而是设计一套能自动驱动Agent运转的循环系统。（[00:00](https://youtu.be/KgiwIEBeOHw?t=0)）
- [[loop-engineering-code-quality-risk]] — 关于AI生成代码质量越来越粗糙的担忧并非空穴来风，在无人值守的循环工程模式下，这个问题会变得更加突出。（[00:00](https://youtu.be/KgiwIEBeOHw?t=0)）
- [[loop-engineering-diy-history]] — 大约一年前，想跑一个自动循环还得自己写一大堆 bash 脚本并长期维护，这类脚本通常只能自己用，很难迁移给他人复用。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[loop-engineering-five-building-blocks]] — 一套完整的循环系统大概由五个基本构建模块组成，目前Claude Code和OpenAI的Codex这两款主流Coding Agent都已经完整具备这五个模块的能力。（[00:00](https://youtu.be/KgiwIEBeOHw?t=0)）
- [[loop-engineering-recursive-goal]] — 在循环工程中，人只需要定义最终目标，AI就会在循环里反复迭代执行直到目标达成，不再需要人工逐轮触发和引导。（[00:00](https://youtu.be/KgiwIEBeOHw?t=0)）
- [[loop-engineering-token-cost-risk]] — 循环工程目前最现实的问题是token成本，不同的使用模式下token消耗量差异非常大，预算有限时必须非常谨慎地规划循环的运行逻辑。（[00:00](https://youtu.be/KgiwIEBeOHw?t=0)）
- [[loop-human-escalation-inbox]] — 所有循环处理不了的复杂问题，就会进入分类收件箱，等待人工处理。（[14:50](https://youtu.be/KgiwIEBeOHw?t=890)）
- [[loop-state-file-continuity]] — 整个循环的核心支柱是状态文件，它记录哪些方案已经尝试过、哪些验证通过了、哪些问题还在处理中，这样第二天早上的自动化任务就可以从今天停下的地方继续推进。（[15:00](https://youtu.be/KgiwIEBeOHw?t=900)）
- [[loop-system-five-modules]] — 一套能稳定运行的循环系统由五个核心功能模块，再加上一个独立的记忆载体共同组成。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[mcp-connectors]] — 如果一个循环只能操作本地文件系统，能做的事情就非常有限；连接器的作用就是让 Agent 能够读取需求跟踪器、查询数据库、调用测试环境接口，甚至在即时通讯工具里发送消息。（[09:03](https://youtu.be/KgiwIEBeOHw?t=543)）
- [[multi-agent-coordination-cost]] — 子Agent会消耗更多token，因为每个Agent都要独立完成模型调用和工具使用，所以子Agent机制不需要到处使用，只在需要二次把关的关键场景开启才划算。（[13:00](https://youtu.be/KgiwIEBeOHw?t=780)）
- [[openai-internal-automation-use-cases]] — OpenAI 内部用自动化能力处理很多重复性日常工作，例如每天自动分类新提交的 issue、汇总持续集成（CI）失败的信息、生成提交记录的简报，以及排查上周新引入的 bug。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
- [[peter-steinberger]] — OpenClaw开发者Peter Steinberger认为，不应该再手动提示Coding Agent，而应该设计让Agent自动运行的循环系统。（[00:00](https://youtu.be/KgiwIEBeOHw?t=0)）
- [[plugins-content-distribution]] — 若要把一个 Skill 共享给多个代码仓库使用，或把好几个相关 Skill 打包到一起，就可以将其封装成一个 Plugin，这一规则在 Codex 和 Claude Code 中都是通用的。（[09:03](https://youtu.be/KgiwIEBeOHw?t=543)）
- [[role-based-model-permission-config]] — 多Agent循环里可以按角色差异化配置：负责安全审查的Agent用能力更强的模型并开启更高推理强度，负责浏览文件的探索型Agent则用速度更快的轻量模型，且只开启只读权限。（[12:04](https://youtu.be/KgiwIEBeOHw?t=724)）
- [[sub-agent-code-review-separation]] — 让写代码的模型自己评审自己的代码往往会出现判断宽松的问题，很难发现自身的逻辑漏洞，而使用第二个拥有不同指令甚至不同模型的 Agent 来评审，就能发现第一个 Agent 忽略掉或主动回避的问题。（[09:03](https://youtu.be/KgiwIEBeOHw?t=543)）
- [[unattended-loop-trusted-verification]] — 验证环节在循环里尤为重要，因为循环很多时候是在没人盯着的情况下运行的，只有拥有一个信得过的验证环节，才能放心让它自己运行。（[12:50](https://youtu.be/KgiwIEBeOHw?t=770)）
- [[unattended-loop-verification-responsibility]] — 一个无人值守运行的循环，同时也是一个无人值守犯错的循环，说到底开发者的工作依然是交付自己亲自确认过可以正常运行的代码，这一点不会因为有了循环而改变。（[15:04](https://youtu.be/KgiwIEBeOHw?t=904)）
