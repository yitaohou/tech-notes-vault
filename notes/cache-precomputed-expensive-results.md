---
title: Caching Precomputed Expensive Results
aliases: []
tags:
- concept
summary: 把计算成本高的操作结果预先计算好并缓存存储，避免重复执行昂贵计算的做法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Caching Precomputed Expensive Results

%% ytkb:def %%
把计算成本高的操作结果预先计算好并缓存存储，避免重复执行昂贵计算的做法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- cache 除了用于限流计数外，也很适合预先计算并存储代价高昂的操作结果，例如编译代码这类昂贵计算可以把结果存入 object storage、再通过 cache 读取，而不必每次重新计算。（[45:11](https://youtu.be/Qa-7iWxDz1A?t=2711)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cache-storage-implementation-options]]
%% ytkb:end %%
