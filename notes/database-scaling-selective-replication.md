---
title: Selective Replication Based on Database Scale
aliases: []
tags:
- concept
summary: 根据各数据库的数据规模和写入压力，选择性决定是否需要引入主从复制，而非对所有数据库一律采用相同的高可用方案。
created: '2026-08-26'
updated: '2026-08-26'
---

# Selective Replication Based on Database Scale

%% ytkb:def %%
根据各数据库的数据规模和写入压力，选择性决定是否需要引入主从复制，而非对所有数据库一律采用相同的高可用方案。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 在 LeetCode 系统设计中，Problems 数据库因数据量小（当前约 4000 条问题）暂不需要 master-slave 复制，但若未来题目规模扩大到数十万，则也需要考虑该架构；而 Submissions 数据库因数据量大、写入频繁，当下就确实需要该架构。（[45:13](https://youtu.be/QBHTbtWSECg?t=2713)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[master-slave-database-replication]]
%% ytkb:end %%
