---
title: Partition Key Selection Based on Query Access Pattern
aliases: []
tags:
- concept
summary: 数据库表的 partition key 应根据实际主要查询访问模式来选择，而不是简单用表的唯一标识符（如自增 ID）作为 partition key。
created: '2026-08-26'
updated: '2026-08-26'
---

# Partition Key Selection Based on Query Access Pattern

%% ytkb:def %%
数据库表的 partition key 应根据实际主要查询访问模式来选择，而不是简单用表的唯一标识符（如自增 ID）作为 partition key。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-data-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- submissions 表选择 competition ID 而非 submission ID 作为 partition key，因为查询主要按某个 competition 聚合并排序其下所有提交，而非按单条 submission ID 查找。（[33:10](https://youtu.be/QBHTbtWSECg?t=1990)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[leaderboard-query-filter-criteria]]
- [[leetcode-submissions-schema]]
%% ytkb:end %%
