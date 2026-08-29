---
title: Single API Consolidation for Leaderboard
aliases: []
tags:
- concept
summary: 把查询、聚合、排名等多个逻辑步骤合并到一个 API 端点里完成，而非拆分成多个独立 API 的设计取舍。
created: '2026-08-26'
updated: '2026-08-26'
---

# Single API Consolidation for Leaderboard

%% ytkb:def %%
把查询、聚合、排名等多个逻辑步骤合并到一个 API 端点里完成，而非拆分成多个独立 API 的设计取舍。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-design]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 排行榜功能不必拆成多个 API（一个查询提交、一个聚合排名、一个返回结果），可以用单个 API 执行一条查询：按 competition ID 筛选出所有提交，再按 user ID 分组统计出排名，视情况也可以拆成两个 API。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[leaderboard-query-flow]]
- [[query-optimization-deferred]]
%% ytkb:end %%
