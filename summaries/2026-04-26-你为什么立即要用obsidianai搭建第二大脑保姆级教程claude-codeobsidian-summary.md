---
video_id: RZEb6FLZSHE
title: 你为什么立即要用Obsidian+AI搭建第二大脑？保姆级教程｜Claude Code+Obsidian
source: '[[2026-04-26-你为什么立即要用obsidianai搭建第二大脑保姆级教程claude-codeobsidian]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: 388a989cb7cc8978d722131f2372e4ccf82543c7b92bdd4c03d4c8d54f89740e
  schema_version: 1
  model: sonnet
  generated_at: '2026-08-26T19:09:10+00:00'
---

## 一句话总结

用 [[obsidian]] 存放本地 Markdown 笔记，配合 [[claude-code]] 直接读写文件夹，通过 [[claude-md-file]]（全局入口）+ [[folder-instructions]]（分文件夹说明）的两层导航机制，搭建一个自动采集输入、AI 辅助整理、按需读取上下文的"无敌第二大脑"([[second-brain-ai]])。

## 核心内容

### 为什么是 Obsidian + AI，而不是 Milanote 或专门的 APP

作者最初的实践是用 [[cursor-editor]] 打开存放视频脚本和读书笔记的本地文件夹，直接让 AI 操作文件内容,体验到"[[folder-as-an-app|folder as an APP]]"的理念（00:00）：很多问题不需要专门开发一个 APP，一个本地文件夹配上 AI 就够了。相比之下，[[milanote]] 的笔记存在云端且结构层层嵌套，AI 很难系统性读取全部内容（00:00）。而 [[obsidian]] 笔记本质上只是本地文件夹里的一堆 Markdown 文件，用 Obsidian 软件打开会有更好的 UI 呈现，且插件生态丰富，这是作者最终选择它的原因（00:00）。[[ai-operates-local-code-files]] 点明了核心逻辑：笔记数据是本地文件，且用代码去编译渲染，这正是 AI 最擅长处理的形式（09:03）。

搭建成本上，Obsidian 软件本身免费，但官方跨设备同步收费；作者的解法是把笔记文件夹放进 [[obsidian-sync-icloud|iCloud]]，免费实现多设备同步（03:00）。

### CLAUDE.md + instructions.md：两层导航机制

整套系统的核心是 [[claude-md-file]]：放在 vault 根目录，Claude 每次运行都会先读取它（00:00）。它主要做两件事——介绍 Claude 的角色定位，以及给出文件夹地图，说明每个文件夹的用途和适用场景（03:00）。还可以写入具体调用规则，比如"写视频内容前先读 context/brand.md""记读书笔记去 reading 文件夹"，避免每次扫描整个笔记库（03:00）。

配合 CLAUDE.md 的是每个文件夹内的 [[instructions-md-file]]，记录该文件夹的具体结构、命名规则和操作方式（03:00）。[[two-layer-navigation-obsidian-claude]] 就是这套机制的名字：CLAUDE.md 中设有强制规则，进入任何文件夹前必须先读该文件夹的 instructions.md（03:00），这样 Claude 只读取当下需要的那一层内容，不必扫描整个库，降低 token 消耗、提升响应速度（03:00）。作者还提到可以借鉴 Anthropic 设计 Claude Code 时用的"[[progressive-disclosure|渐进式披露]]"原理来理解这种按需读取的做法（09:03），这与 [[on-demand-context-retrieval]] 的思路一致——笔记库越大，按需索取上下文而不是全部读取就越关键（12:04）。

[[context-folder]] 是整套系统里最核心的一个文件夹，存放作者自己的身份、目标和表达风格信息，AI 每次运行先读这里，避免每次都要重新自我介绍（00:00）。

### 自动化输入管道：让内容自己流进笔记库

为了降低存储笔记的操作成本、避免半途而废，作者搭建了全自动的 [[automated-input-pipeline]]，让信息自动流入笔记库而不需要手动整理（03:00）。具体工具包括：

- [[obsidian-web-clipper]]：一键抓取网页标题、链接、作者和正文，保存为 Markdown（03:00）。其 [[web-clipper-reading-mode|阅读模式]] 特别适合长视频类学习内容，可以边看视频边看字幕文本，点击时间戳还能自动跳转到视频对应片段（03:00）。
- [[obsidian-youtube-plugin]]：点击 add to obsidian 按钮即可一键导入 YouTube 视频内容（06:02）。
- [[apple-books-highlights-plugin]]：把 Apple Books 中的划线一次性导入 Obsidian，这也让作者的阅读习惯从纸质书转向了电子书（06:02）。
- [[ios-shortcuts-app]] + [[iphone-action-button]]：在 Shortcuts 里设置语音转录并自动追加到 [[obsidian-daily-notes|Daily Notes]] 的工作流，绑定到 Action Button 后随时按一下就能捕捉灵感（06:02）。

这背后是 [[second-brain]] 的一个原则——集中性输入、发散性输出：人一天会产生几十个想法，需要随时捕捉一闪而过的灵感（06:02）。语音记录的碎碎念会带时间戳自动追加到当天 Daily Notes，作者会在 instructions 中提前告诉 AI 这些带时间戳的内容是随手记录，方便之后二次整理创作（06:02）。

### Daily Notes 与 Canvas：跨 session 的记忆与发散思维

[[daily-notes-obsidian]] 承担了跨 session 记忆的作用：每天工作结束时让 Claude Code 把当天完成的工作和待跟进事项写入当天笔记；下次开新 session 时，只需读最近几天的 Daily Notes 就能知道之前做了什么、卡在哪、还需要做什么，无需读整个库（12:04）。

对于发散性思维导图需求，[[obsidian-canvas]] 替代了 Milanote 的角色（06:02），其本质是本地 JSON 文件，可以在里面自由绘图（09:03）。

### 接入 AI 的两种方式与迁移实践

Obsidian 里接入 AI 有两种方式：一是安装 [[obsidian-terminal-plugin]]，在 Obsidian 界面内直接打开终端调用 Claude，无需切到外部终端（09:03）；二是配置 [[obsidian-ai-chat-plugin]]，直接在界面内与 AI 对话（09:03）。日常处理笔记的常见做法是把整个笔记文件夹拖给 Claude Code 并开启 [[yolo-mode-claude-code|YOLO 模式]]，让它执行操作时不反复询问权限（09:03）。迁移旧笔记时，甚至可以把旧软件界面截屏发给 [[claude-code]]，让它照着截图内容在新系统里复刻文件结构（09:03）。

进阶用法上，可以把 [[claude-skills]] 存放到 Obsidian 的 skills 文件夹，让 Claude 直接指向该目录，这样 skill 里的参考文档能随笔记库内容持续优化而实时更新（12:04），这也呼应了 [[obsidian-second-brain]] 的迭代属性。此外用 [[obsidian-cli|Obsidian 官方 CLI]] 操作笔记可以进一步减少 Claude 的 token 消耗（12:04）。

### 理念源头与长期价值

这套方法论呼应了 [[andrej-karpathy]] 提出的用 LLM 结构化个人原始信息、构建个人知识系统的理念（12:04）：人每天接触大量杂乱的原始信息（推文、文章、会议记录、读书笔记），用 LLM 本地结构化编译，再用 Obsidian+AI 查看操作，就能构建一个随时间积累越来越强的 [[personal-knowledge-system-karpathy|个人知识系统]]（12:04）。

作者强调，第二大脑系统的实际效用取决于存放内容的质量和丰富度，而不仅仅是工具搭建方式本身（03:00）。经过几个月持续积累后，打开 Claude 时它能基于笔记内容"认出"使用者本人，体现了 [[ai-context-personalization]]（15:04）。这样搭建出的 [[local-private-knowledge-base]] 是完全本地化、私有的资产，不是某家 AI 公司卖的功能，任何 AI 都可以接入使用（15:04）。在 AI 功能快速迭代的当下，慢慢积累这样的 [[personal-knowledge-asset]] 是不可替代的长期价值方向（15:04）。

## 值得记住的细节

- 00:00 设计 [[folder-structure-for-ai|文件夹结构]] 没有标准答案，核心原则是让 AI 知道该去哪个文件夹找什么信息，而不只是方便自己导航。
- 03:00 CLAUDE.md 中的强制规则：进入任何文件夹前必须先读该文件夹的 instructions.md（[[two-layer-navigation-obsidian-claude]]）。
- 03:00 Obsidian 官方同步收费，作者用 iCloud 免费替代（[[obsidian-sync-icloud]]）。
- 06:02 iPhone Action Button 绑定 Shortcuts 快捷指令，一键开始语音记录灵感。
- 09:03 常规操作方式：把整个笔记文件夹拖给 Claude Code，开启 YOLO 模式，减少权限确认打断。
- 09:03 迁移旧笔记软件时可直接截图发给 Claude Code，让其照图复刻文件结构。
- 12:04 用 Obsidian 官方 CLI 操作笔记可降低 token 消耗。
- 12:04 每天工作结束让 Claude 把当天进展写入 Daily Notes，新 session 只需读最近几天笔记即可恢复上下文，无需通读全库。
- 12:04 Claude Skills 放入 Obsidian 的 skills 文件夹，参考文档随笔记库更新自动同步。

## 这个视频适合谁 / 可以跳过什么

适合：已经在用或打算用 Obsidian 做笔记、想用 AI（Claude Code/Codex）自动化整理和检索个人知识、对"第二大脑"工作流感兴趣、愿意折腾插件和自动化输入管道的人。

可以跳过：如果只想要一个开箱即用的笔记软件、不打算配置 CLAUDE.md/instructions.md 体系或安装终端类插件，本视频的核心方法论（两层导航、渐进式披露、自动化输入管道）价值有限，可以只看 00:00 和 15:04 了解整体理念即可。
