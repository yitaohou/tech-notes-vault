---
title: In-Memory Cache vs Distributed Cache
aliases: []
tags:
- concept
summary: 缓存架构选择中的一对权衡方案：单机进程内的 in-memory cache 与跨节点共享的 distributed cache。
created: '2026-08-26'
updated: '2026-08-26'
---

# In-Memory Cache vs Distributed Cache

%% ytkb:def %%
缓存架构选择中的一对权衡方案：单机进程内的 in-memory cache 与跨节点共享的 distributed cache。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 排行榜缓存可以选择使用 in-memory cache（单机内存缓存），也可以选择 distributed cache（分布式缓存），两者在架构设计上是可权衡的替代方案。（[39:13](https://youtu.be/QBHTbtWSECg?t=2353)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cache-framework-choice]]
- [[leaderboard-caching]]
%% ytkb:end %%
