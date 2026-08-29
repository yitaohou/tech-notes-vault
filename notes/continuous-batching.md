---
title: Continuous Batching
aliases: []
tags:
- concept
summary: continuous batching 允许请求一旦处理完成就立即返回结果，同时不断加入新请求以维持批次规模。
created: '2026-08-26'
updated: '2026-08-26'
---

# Continuous Batching

%% ytkb:def %%
continuous batching 允许请求一旦处理完成就立即返回结果，同时不断加入新请求以维持批次规模。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- continuous batching 让已完成的响应可以立即返回，同时不断补入新请求维持批次大小，能提供最佳用户体验，但实现更复杂。（[66:06](https://youtu.be/JV3pL1_mn2M?t=3966)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dynamic-batching]]
- [[request-batching]]
%% ytkb:end %%
