---
title: CLAUDE.md File
aliases: []
tags:
- concept
summary: CLAUDE.md 是放在知识库根目录、用于向 Claude 说明其角色定位并提供文件夹地图的配置文件。
created: '2026-08-26'
updated: '2026-08-26'
---

# CLAUDE.md File

%% ytkb:def %%
CLAUDE.md 是放在知识库根目录、用于向 Claude 说明其角色定位并提供文件夹地图的配置文件。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:RZEb6FLZSHE %%
### 来自 [[2026-04-26-你为什么立即要用obsidianai搭建第二大脑保姆级教程claude-codeobsidian]]
- CLAUDE.md 文件主要做两件事：介绍 Claude 的角色定位（你是谁、在做什么），以及给出文件夹地图，说明每个文件夹的用途和适用场景。（[03:00](https://youtu.be/RZEb6FLZSHE?t=180)）
- 可以在 CLAUDE.md 中写入具体调用规则，例如写视频内容前要先读 context brand.md 文件，记读书笔记时要去 reading 文件夹查找，从而避免每次都扫描整个笔记库。（[03:00](https://youtu.be/RZEb6FLZSHE?t=180)）
- 在 vault 根目录放置一个 CLAUDE.md 文件，作为整个第二大脑系统的入口，Claude 每次运行都会先读取它。（[00:00](https://youtu.be/RZEb6FLZSHE?t=0)）
- 作者为笔记库设置了 CLAUDE.md 文档，Claude 每次执行任务时会先读取这个文档，再进入相应文件夹读取该文件夹内的 instructions 文件，最后再执行具体任务。（[09:03](https://youtu.be/RZEb6FLZSHE?t=543)）
- 通过给 Claude Code 提供一个 claude.md 文档，说明整个笔记库文件夹结构，AI 不需要每次直接读取整个笔记库。（[12:04](https://youtu.be/RZEb6FLZSHE?t=724)）
%% ytkb:end %%

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- 以前写 CLAUDE.md 或系统提示词时，总想把项目里所有的坑、规范和代码审查标准都写成百科全书式地塞进去。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- 早期 Claude Code 官方建议开发者用快捷键手动把重要的经验教训记录进 CLAUDE.md 文件，如同带实习生时每次犯错都要手动记小本子，下次干活前再让其查看。（[06:01](https://youtu.be/Lle_EJljIoo?t=361)）
- 好的上下文架构要求 CLAUDE.md 只保留模型无法通过扫描代码库自行获知的核心项目信息（如项目陷阱），不必写模型扫一眼就能懂的废话。（[09:55](https://youtu.be/Lle_EJljIoo?t=595)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[automatic-memory-claude]]
- [[claude-code]]
- [[context-engineering]]
- [[context-folder]]
- [[context-window-limits-large-models]]
- [[folder-instructions]]
- [[instructions-md-file]]
- [[on-demand-context-retrieval]]
- [[progressive-disclosure]]
- [[two-layer-navigation-obsidian-claude]]
%% ytkb:end %%
