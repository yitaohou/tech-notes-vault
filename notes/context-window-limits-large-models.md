---
title: Context Window Limits for Large Models
aliases: []
tags:
- concept
summary: 即便模型拥有百万 token 级别的大上下文窗口，塞入过多无关信息依然会干扰模型注意力，并大幅增加 token 成本。
created: '2026-08-26'
updated: '2026-08-26'
---

# Context Window Limits for Large Models

%% ytkb:def %%
即便模型拥有百万 token 级别的大上下文窗口，塞入过多无关信息依然会干扰模型注意力，并大幅增加 token 成本。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- 哪怕新模型拥有百万 Token 级别的上下文窗口，塞入太多无关信息依然会干扰其注意力，还会大幅增加 token 成本。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-md-file]]
- [[progressive-disclosure]]
%% ytkb:end %%
