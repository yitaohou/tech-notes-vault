---
title: Tensor Parallelism
aliases: []
tags:
- concept
summary: tensor parallelism 是 model parallelism 的一种方式，把单个运算操作拆分成更小的部分分布执行。
created: '2026-08-26'
updated: '2026-08-26'
---

# Tensor Parallelism

%% ytkb:def %%
tensor parallelism 是 model parallelism 的一种方式，把单个运算操作拆分成更小的部分分布执行。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- tensor parallelism 将模型中的运算操作拆分成更小的部分分布到不同设备上执行，是 model parallelism 的实现方式之一。（[66:06](https://youtu.be/JV3pL1_mn2M?t=3966)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[model-parallelism]]
%% ytkb:end %%
