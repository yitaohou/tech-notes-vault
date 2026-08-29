---
title: STOP (Self-Taught Optimizer)
aliases: []
tags:
- concept
summary: 一种通过迭代让模型改进自身 Harness/机制来提升下游任务表现的递归自我改进方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# STOP (Self-Taught Optimizer)

%% ytkb:def %%
一种通过迭代让模型改进自身 Harness/机制来提升下游任务表现的递归自我改进方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- STOP 框架下，若把基础模型换成能力更弱的 GPT-3.5 或 Mixtral，随迭代次数增加性能反而下降，说明光有递归改进结构不足以带来提升，基础模型必须具备足够强的能力才能真正改进机制本身。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-harness]]
%% ytkb:end %%
