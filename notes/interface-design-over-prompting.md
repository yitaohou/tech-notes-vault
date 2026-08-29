---
title: Interface Design over Prompting
aliases: []
tags:
- concept
summary: 与其用大量提示词描述工具用法，不如把工具的输入输出接口设计得更清晰、更具表达力，让模型自行理解如何使用。
created: '2026-08-26'
updated: '2026-08-26'
---

# Interface Design over Prompting

%% ytkb:def %%
与其用大量提示词描述工具用法，不如把工具的输入输出接口设计得更清晰、更具表达力，让模型自行理解如何使用。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- 针对新模型的最佳实践是设计更好的工具接口参数，而不是写长篇说明去解释工具的用法。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[enum-parameter-design]]
- [[few-shot-examples-limit-exploration]]
%% ytkb:end %%
