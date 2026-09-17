---
video_id: U6ZHJPNvlxU
url: https://www.youtube.com/watch?v=U6ZHJPNvlxU
title: 介绍 Herdr 后，评论区为什么都在推荐 Orca？
channel: 大力Thinking
published: '2026-09-14'
duration: 08:38
transcript_origin: subs
tags:
- video
---

# 介绍 Herdr 后，评论区为什么都在推荐 Orca？

摘要: [[2026-09-14-介绍-herdr-后评论区为什么都在推荐-orca-summary|完整摘要]]

## 知识点

- [[element-picker-precision-vs-natural-language]] — 相比用自然语言描述网页元素（如“把右上角的蓝色按钮改一改”），用元素抓取功能获取的精确技术信息能让 AI 更准确地定位并修改指定元素。（[03:00](https://youtu.be/U6ZHJPNvlxU?t=180)）
- [[git-worktree-multi-agent-isolation]] — Orca 正是采用 Git worktree 机制为每个并行运行的 Agent 提供独立工作目录，这是其区别于普通多终端工具的核心技术基础。（[06:01](https://youtu.be/U6ZHJPNvlxU?t=361)）
- [[orca-ade]] — Orca 在其 GitHub 页面上把自己定位为 ADE（Agent Development Environment），是相对于传统 IDE 提出的新范式，ADE 中的 A 代表 Agent，即专为 AI 编程 Agent 设计的开发环境。（[00:00](https://youtu.be/U6ZHJPNvlxU?t=0)）
- [[orca-agent-agnostic-host]] — Orca 并不是一个新模型，也不是另一个 Codex 或 Claude Code，而是可以把用户原本熟悉的 Codex、Claude Code、Cursor、Gemini、OpenCode 等任意终端 Agent 放进来运行的宿主环境。（[00:00](https://youtu.be/U6ZHJPNvlxU?t=0)）
- [[orca-agent-lifecycle-management]] — Orca 除了帮用户开启多个终端和多个 Agent 外，还持续管理这些 Agent 的工作状态，而不只是充当一个简单的启动入口。（[03:00](https://youtu.be/U6ZHJPNvlxU?t=180)）
- [[orca-agent-status-indicator]] — Orca 的每个标签旁会显示状态指示灯，当某个 Agent 正在运行时指示灯会发生变化，使用户即便切换到其他 Agent 标签，也能了解另一个 Agent 的运行状态。（[03:00](https://youtu.be/U6ZHJPNvlxU?t=180)）
- [[orca-cli-gui-hybrid]] — 元素抓取这类可视化功能在 Codex 等命令行版 Agent 软件中已有内置，但如果既想用命令行版 Agent、又想体验可视化功能，Orca 可以把两者结合在一起使用。（[03:00](https://youtu.be/U6ZHJPNvlxU?t=180)）
- [[orca-diff-inline-comment-workflow]] — 发送评论时可选择只针对当前文件，或把所有尚未发送的评论一并打包发给同一个 Agent。（[06:01](https://youtu.be/U6ZHJPNvlxU?t=361)）
- [[orca-diff-review]] — Agent 完成代码改动后，Orca 会展开一个目录树展示所有相关改动文件，用户可逐一点击查看具体的代码或文档差异，供合并前审核。（[03:00](https://youtu.be/U6ZHJPNvlxU?t=180)）
- [[orca-element-picker]] — 点击 Orca 的抓取页面元素按钮后，用户可以在内置浏览器中选中某个网页元素并点击 Copy，粘贴到对话框中会自动带出该元素的 CSS 样式、HTML、大小和标签选择器等详尽描述。（[03:00](https://youtu.be/U6ZHJPNvlxU?t=180)）
- [[orca-embedded-browser]] — 如果开发的是前端项目，可以直接在 Orca 内部打开该项目对应的网页，并在其中新建浏览器选项卡访问指定网站，无需离开 Orca 环境。（[03:00](https://youtu.be/U6ZHJPNvlxU?t=180)）
- [[orca-floating-auxiliary-window]] — 该悬浮窗口在用户切换到其他任务查资料或临时提问时不会消失，可以与主工作区并存。（[06:01](https://youtu.be/U6ZHJPNvlxU?t=361)）
- [[orca-git-visualization]] — 在 Orca 的 Diff 视图中点击 Git 图标，可以直接打开内置的 Git 可视化界面，无需切换到外部 Git 工具。（[03:00](https://youtu.be/U6ZHJPNvlxU?t=180)）
- [[orca-mit-license]] — 作者认为 Orca 作为一个成熟度很高的 AI 工作台项目，采用 MIT 开源协议是很了不起的一点。（[06:01](https://youtu.be/U6ZHJPNvlxU?t=361)）
- [[orca-mobile-pairing]] — 手机与电脑处于同一局域网时可直接扫码配对；若不在同一局域网，则需注册账号后通过互联网进行远程配对。（[06:01](https://youtu.be/U6ZHJPNvlxU?t=361)）
- [[orca-multi-agent-tabs]] — Orca 允许在同一项目下同时创建多个工作区标签，各标签可分别绑定不同 Agent（例如一个绑定 Codex、另一个绑定 Claude Code），彼此独立运行互不干扰，最终由使用者自行决定把哪个标签的工作结果合并回主工作区。（[03:00](https://youtu.be/U6ZHJPNvlxU?t=180)）
- [[orca-project-import-methods]] — 在 Orca 中添加项目支持三种方式：浏览本地文件夹、选择已有 Git 仓库，或从远端克隆一个新项目。（[00:00](https://youtu.be/U6ZHJPNvlxU?t=0)）
- [[orca-terminal-split-view]] — 除了 Codex 和 Claude Code，Orca 还可以在标签里打开一个新终端，并支持把终端窗口拖到旁边与 Agent 面板并排显示，方便同时操作两者。（[03:00](https://youtu.be/U6ZHJPNvlxU?t=180)）
- [[orca-unified-workspace]] — Orca 做的核心事情，是把 Agent、代码、终端、浏览器、Git 分支和代码审查整合到同一个工作环境里。（[00:00](https://youtu.be/U6ZHJPNvlxU?t=0)）
- [[orca-workspace-redesign-philosophy]] — 以 Worktree 为基础的多 Agent 管理方式，只有在同时使用 Codex、Claude Code 等多个 Agent 并行处理多个开发任务时才真正值得体验；如果平时只开一个 Agent 做简单修改，这套体系会显得偏重。（[06:01](https://youtu.be/U6ZHJPNvlxU?t=361)）
