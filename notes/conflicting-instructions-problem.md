---
title: Conflicting Instructions Problem
aliases: []
tags:
- concept
summary: 系统提示词与用户指令相互矛盾时，模型无法判断该遵循哪一方，从而陷入困惑的问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# Conflicting Instructions Problem

%% ytkb:def %%
系统提示词与用户指令相互矛盾时，模型无法判断该遵循哪一方，从而陷入困惑的问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-prompt-engineering]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- 当系统提示词说「不要写注释」而用户要求「请留下适当的文档」时，模型会因指令自相矛盾而困惑，不知该听谁的。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-code]]
- [[hard-coded-prompt-rules]]
%% ytkb:end %%
