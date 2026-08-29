---
title: Code Style Matching Instruction
aliases: []
tags:
- concept
summary: 新版系统提示词用「编写与周围代码风格一致的代码」一句话替代大量硬性规则，让模型自行匹配注释密度、命名和惯用语法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Code Style Matching Instruction

%% ytkb:def %%
新版系统提示词用「编写与周围代码风格一致的代码」一句话替代大量硬性规则，让模型自行匹配注释密度、命名和惯用语法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-prompt-engineering]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- 新版提示词只用一句话「编写与周围代码风格一致的代码」，要求模型匹配现有代码的注释密度、命名和惯用语法，取代了大量硬性规则。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- 这种简化提示词的方式说明新模型已具备类似高级工程师的上下文感知能力，能自行判断代码规范，无需逐条被告知该怎么做。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-code]]
- [[hard-coded-prompt-rules]]
%% ytkb:end %%
