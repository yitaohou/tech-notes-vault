---
title: Dynamic Batching
aliases: []
tags:
- concept
summary: dynamic batching 设定一个最大等待时间窗口，在批次凑满或超时任一条件满足时就开始处理。
created: '2026-08-26'
updated: '2026-08-26'
---

# Dynamic Batching

%% ytkb:def %%
dynamic batching 设定一个最大等待时间窗口，在批次凑满或超时任一条件满足时就开始处理。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- dynamic batching 通过设置最大时间窗口，在批次已满或时间限制已到这两个条件中任一满足时就处理该批次，从而提供更稳定的延迟保证。（[66:06](https://youtu.be/JV3pL1_mn2M?t=3966)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[continuous-batching]]
- [[request-batching]]
- [[static-batching]]
%% ytkb:end %%
