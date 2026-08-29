---
title: Compute-Bound vs Memory-Bound Optimization
aliases: []
tags:
- concept
summary: 根据工作负载属于计算密集型还是内存密集型，选择不同硬件优化重点的原则。
created: '2026-08-26'
updated: '2026-08-26'
---

# Compute-Bound vs Memory-Bound Optimization

%% ytkb:def %%
根据工作负载属于计算密集型还是内存密集型，选择不同硬件优化重点的原则。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 对于 compute-bound 的工作负载应优先选择 flops 更高的芯片，对于 memory-bound 的工作负载则应侧重更高的内存带宽和更大的内存容量。（[63:05](https://youtu.be/JV3pL1_mn2M?t=3785)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[model-bandwidth-utilization]]
- [[model-flops-utilization]]
%% ytkb:end %%
