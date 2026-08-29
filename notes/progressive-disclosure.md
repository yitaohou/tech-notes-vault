---
title: Progressive Disclosure（渐进式披露）
aliases: []
tags:
- concept
summary: 渐进式披露是 Anthropic 设计 Claude Code 的核心原理之一：AI 不会一次性读取全部内容，而是按需、分层地逐步获取所需信息，从而控制上下文和
  token 消耗。
created: '2026-08-26'
updated: '2026-08-26'
---

# Progressive Disclosure（渐进式披露）

%% ytkb:def %%
渐进式披露是 Anthropic 设计 Claude Code 的核心原理之一：AI 不会一次性读取全部内容，而是按需、分层地逐步获取所需信息，从而控制上下文和 token 消耗。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:RZEb6FLZSHE %%
### 来自 [[2026-04-26-你为什么立即要用obsidianai搭建第二大脑保姆级教程claude-codeobsidian]]
- 针对“让 AI 读取整个笔记库会不会消耗大量 token”的疑问，作者提出可以借鉴 Anthropic 设计 Claude Code 时采用的“渐进式披露”原理来理解和优化。（[09:03](https://youtu.be/RZEb6FLZSHE?t=543)）
%% ytkb:end %%

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- 从「全盘托出」转向「按需加载」被认为是这次提示词理念转变中，对开发 AI Agent 影响最大的一点。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- 渐进式披露的具体做法是把代码审查规则、数据库迁移注意事项等分别写成独立的 Skill，模型只在真正需要执行相应任务时才去调用对应 Skill 读取规则，而不是把所有规则都塞进主提示词。（[06:01](https://youtu.be/Lle_EJljIoo?t=361)）
- 应将大段规范拆分成按需加载的模块，而不是一次性塞给模型，这是渐进式披露思路在上下文设计上的具体应用。（[10:10](https://youtu.be/Lle_EJljIoo?t=610)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-code]]
- [[claude-md-file]]
- [[claude-skills]]
- [[context-engineering]]
- [[context-window-limits-large-models]]
- [[on-demand-tool-loading]]
%% ytkb:end %%
