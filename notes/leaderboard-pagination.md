---
title: Leaderboard Pagination
aliases: []
tags:
- concept
summary: 为排行榜接口设计分页机制，限制单页返回的选手数量，以避免一次性返回过多数据。
created: '2026-08-26'
updated: '2026-08-26'
---

# Leaderboard Pagination

%% ytkb:def %%
为排行榜接口设计分页机制，限制单页返回的选手数量，以避免一次性返回过多数据。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 排行榜接口需要支持分页，以便每页只展示有限数量的选手，例如默认限制为 100 条，且该限制可根据需要调整。（[18:07](https://youtu.be/QBHTbtWSECg?t=1087)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[leaderboard-api-design]]
%% ytkb:end %%
