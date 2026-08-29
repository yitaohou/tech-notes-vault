---
title: Roofline Chart
aliases: []
tags:
- concept
summary: 一种通过 profiling 工具（如 Nvidia Insight）生成的图表，用于判断某个 workload 是 compute bound
  还是 memory bandwidth bound。
created: '2026-08-26'
updated: '2026-08-26'
---

# Roofline Chart

%% ytkb:def %%
一种通过 profiling 工具（如 Nvidia Insight）生成的图表，用于判断某个 workload 是 compute bound 还是 memory bandwidth bound。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 可以用 Nvidia Insight 等 profiling 工具生成 roofline chart，来判断某个 workload 究竟是 compute bound 还是 memory bandwidth bound。（[60:04](https://youtu.be/JV3pL1_mn2M?t=3604)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[compute-bound-bottleneck]]
- [[memory-bandwidth-bound-bottleneck]]
%% ytkb:end %%
