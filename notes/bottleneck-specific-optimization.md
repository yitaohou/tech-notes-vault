---
title: Bottleneck-Specific Optimization Strategy
aliases: []
tags:
- concept
summary: 不同类型的推理瓶颈需要用不同的优化手段来针对性解决。
created: '2026-08-26'
updated: '2026-08-26'
---

# Bottleneck-Specific Optimization Strategy

%% ytkb:def %%
不同类型的推理瓶颈需要用不同的优化手段来针对性解决。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- compute bound workload 更适合用算力更强的芯片或把任务分布到多颗芯片上来优化，而 memory bandwidth bound workload 更适合用内存带宽更高的芯片来优化。（[60:04](https://youtu.be/JV3pL1_mn2M?t=3604)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[compute-bound-bottleneck]]
- [[memory-bandwidth-bound-bottleneck]]
%% ytkb:end %%
