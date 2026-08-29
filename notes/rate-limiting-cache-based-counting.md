---
title: Cache-Based Rate Limit Counting
aliases: []
tags:
- concept
summary: 利用 cache 的 key-value 存储和内存读写速度，实时记录并统计每个用户在时间窗口内请求次数的 rate limiting 实现方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Cache-Based Rate Limit Counting

%% ytkb:def %%
利用 cache 的 key-value 存储和内存读写速度，实时记录并统计每个用户在时间窗口内请求次数的 rate limiting 实现方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 因为 cache 是运行在 RAM 中的 key-value storage，读写速度快，非常适合用来实时统计每个用户在时间窗口内（如最近一分钟内发起了五次请求）的请求次数。（[45:11](https://youtu.be/Qa-7iWxDz1A?t=2711)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[in-memory-vs-distributed-cache]]
- [[rate-limiting]]
%% ytkb:end %%
