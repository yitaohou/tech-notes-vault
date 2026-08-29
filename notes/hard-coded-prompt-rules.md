---
title: Hard-coded Prompt Rules
aliases: []
tags:
- concept
summary: 旧版系统提示词中为了堵死边界条件而写的一系列硬性规则，例如强制规定注释密度和文档格式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Hard-coded Prompt Rules

%% ytkb:def %%
旧版系统提示词中为了堵死边界条件而写的一系列硬性规则，例如强制规定注释密度和文档格式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-prompt-engineering]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- Claude Code旧版系统提示词中明确规定「默认不写注释」「最多只能写一行简短注释」等硬性规则，试图堵死所有边界条件。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- 硬性规则在遇到复杂算法逻辑或用户有自己的代码规范时，会导致 AI 写出的代码难以维护。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-code]]
- [[code-style-matching-instruction]]
- [[conflicting-instructions-problem]]
%% ytkb:end %%
