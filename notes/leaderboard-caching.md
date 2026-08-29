---
title: Leaderboard Caching
aliases: []
tags:
- concept
summary: 周期性计算排行榜结果并存入缓存，使读取请求优先命中缓存而非直接查询数据库的优化方案。
created: '2026-08-26'
updated: '2026-08-26'
---

# Leaderboard Caching

%% ytkb:def %%
周期性计算排行榜结果并存入缓存，使读取请求优先命中缓存而非直接查询数据库的优化方案。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 为降低轮询数据库带来的负载，可以引入缓存机制：周期性计算排行榜并将结果存入缓存，读取请求优先从缓存获取，从而减少数据库负载，但代价是排行榜数据不是严格实时的，本质上仍是在定期查询数据库后缓存结果。（[39:13](https://youtu.be/QBHTbtWSECg?t=2353)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[leaderboard-polling]]
%% ytkb:end %%
