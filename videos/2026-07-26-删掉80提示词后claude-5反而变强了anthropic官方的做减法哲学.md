---
video_id: Lle_EJljIoo
url: https://www.youtube.com/watch?v=Lle_EJljIoo
title: 删掉80%提示词后，Claude 5反而变强了？Anthropic官方的做减法哲学
channel: Why QQ
published: '2026-07-26'
duration: '12:02'
transcript_origin: subs
tags:
- video
---

# 删掉80%提示词后，Claude 5反而变强了？Anthropic官方的做减法哲学

摘要: [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学-summary|完整摘要]]

## 知识点

- [[api-design-as-documentation]] — 好的 API 设计本身就是最好的文档，与其花几百字提示词解释一个糟糕接口，不如把工具的输入输出结构设计得更清晰、更具表达力。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- [[automatic-memory-claude]] — Claude 现在能在工作过程中自动总结经验教训并保存有用信息，下次工作时自动调取，开发者不再需要充当手动记小本子的角色。（[06:01](https://youtu.be/Lle_EJljIoo?t=361)）
- [[avoid-redundant-instructions]] — 同一条要求不用在系统提示词和工具描述里反复强调，放在最相关的位置说清楚一次就够了。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- [[chat-based-coding-context]] — ChatGPT 和早期 Claude 时代，开发者开始用对话的方式让 AI 写代码，这时上下文变成了对话历史。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
- [[claude-5]] — Claude 5 的输出价格大约是 Opus 4.5 的两倍，裸用其处理复杂项目时这是需要掂量的成本因素。（[06:01](https://youtu.be/Lle_EJljIoo?t=361)）
- [[claude-md-file]] — 以前写 CLAUDE.md 或系统提示词时，总想把项目里所有的坑、规范和代码审查标准都写成百科全书式地塞进去。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- [[code-style-matching-instruction]] — 新版提示词只用一句话「编写与周围代码风格一致的代码」，要求模型匹配现有代码的注释密度、命名和惯用语法，取代了大量硬性规则。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- [[conflicting-instructions-problem]] — 当系统提示词说「不要写注释」而用户要求「请留下适当的文档」时，模型会因指令自相矛盾而困惑，不知该听谁的。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- [[context-dilution]] — Anthropic 工程师发现，太多无关上下文会稀释模型注意力，过去『保姆式』的提示词反而成了限制模型发挥的枷锁。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
- [[context-ecosystem-claude-code]] — 到 Opus 5、Sonnet 5 配合 Claude Code 这种级别的 Agent，上下文的定义被再次刷新：不再是简单的文本堆砌，而是一个包含系统提示词、动态技能、本地配置、自动记忆和丰富引用的复杂生态系统。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
- [[context-engineering]] — Anthropic 把构建和管理系统提示词、动态技能、本地配置、自动记忆和丰富引用这个复杂生态系统的过程，称为『上下文工程』（Context Engineering）。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
- [[context-window-limits-large-models]] — 哪怕新模型拥有百万 Token 级别的上下文窗口，塞入太多无关信息依然会干扰其注意力，还会大幅增加 token 成本。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- [[copilot-code-completion]] — 最早的 Copilot 只是单纯的代码补全工具，用户写个注释它就补一段代码，当时的上下文只是当前打开的文件，最多加上几个相邻文件。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
- [[cursor-editor]] — Cursor 会把整个代码库做成索引，在用户提问时检索出相关代码片段喂给模型，把上下文从对话历史扩展到了项目级别。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
- [[enum-parameter-design]] — Todo 工具把状态参数定义为 pending、inprogress、completed 三个枚举值，模型看到后就能自己理解如何调用，无需长篇文字说明。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- [[few-shot-examples-limit-exploration]] — 对最新模型而言，few-shot 示例可能限制其探索空间，如果给出的例子只展示基础用法，模型可能永远学不会组合使用高级参数。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- [[few-shot-prompting-tool-use]] — 以前教 AI 使用工具的稳妥方法是给它喂大量 few-shot 示例，逐一说明每种场景下的具体输入格式，例如查天气或更新任务状态该怎么写。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- [[hard-coded-prompt-rules]] — Claude Code旧版系统提示词中明确规定「默认不写注释」「最多只能写一行简短注释」等硬性规则，试图堵死所有边界条件。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- [[hardcoded-prompt-rules-limitation]] — 模型能力变强以后，旧时代为约束其行为而写的硬性提示词规则可能开始限制模型自身的判断。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
- [[interface-design-over-prompting]] — 针对新模型的最佳实践是设计更好的工具接口参数，而不是写长篇说明去解释工具的用法。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- [[model-routing-by-complexity]] — 工程上常见做法是按任务复杂度分流：简单补全和基础问答用小模型，只有跨多文件、需要长程推理的硬核重构才调用顶配模型。（[09:02](https://youtu.be/Lle_EJljIoo?t=542)）
- [[on-demand-tool-loading]] — 工具的定义也可以像规则一样按需加载：Agent 起初只知道有这么个工具，等真正需要用到时才去加载该工具的具体定义，类似主函数保持干净、业务逻辑封装进模块按需调用。（[06:01](https://youtu.be/Lle_EJljIoo?t=361)）
- [[paradigm-shift-human-designs-context]] — 未来 AI 编程考验的不是与 AI 聊天的技巧，而是对系统架构的理解，以及能否为 AI 构建清晰、高效、无歧义的工作环境。（[10:25](https://youtu.be/Lle_EJljIoo?t=625)）
- [[progressive-disclosure]] — 从「全盘托出」转向「按需加载」被认为是这次提示词理念转变中，对开发 AI Agent 影响最大的一点。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- [[prompt-engineering]] — 早期观点认为写好 Prompt 是一门需要学习各种咒语和技巧的玄学，甚至催生了「提示词工程师」这一岗位。（[09:40](https://youtu.be/Lle_EJljIoo?t=580)）
- [[rich-context-references]] — 新模型能够直接处理 HTML 格式的 UI 原型作为参考资料，比用几百字描述界面长什么样效果更好。（[06:01](https://youtu.be/Lle_EJljIoo?t=361)）
- [[rubrics-evaluation]] — 可以用动态工作流启动一个专门的验证 Agent，把 Rubrics 喂给它，让它评估主 Agent 写出的代码是否符合预定义的标准，例如什么样的 API 设计才算优雅。（[06:01](https://youtu.be/Lle_EJljIoo?t=361)）
- [[safety-classifier-claude]] — 部分命中网络安全或生物相关内容的请求可能被安全分类器转交给 Opus 处理，在 API 场景下也可能被直接拒绝。（[09:02](https://youtu.be/Lle_EJljIoo?t=542)）
- [[sonnet-5-stripe-migration-case]] — 根据 Anthropic 发布页援引的 Stripe 早期测试，Sonnet 5 曾在一天内完成一个约 5000 万行 Ruby 代码库的全库迁移，Stripe 估计如果由团队手工完成需要两个多月。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
- [[system-prompt-reduction-claude-code]] — Anthropic 工程师 Thariq Shihipar 透露，针对 Opus 5 和 Sonnet 5 两个新模型，Claude Code 的系统提示词被缩短了超过 80%。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
- [[thariq-shihipar]] — Thariq Shihipar 在文章中把 Claude Code 系统提示词此次变化的原因总结成了几个核心转变。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
- [[verbose-prompt-paradigm]] — 从 GPT-3 时代开始，行业里流行的做法是提示词写得越详细越好，把 AI 当成听不懂人话的实习生，手把手教它每一步。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
