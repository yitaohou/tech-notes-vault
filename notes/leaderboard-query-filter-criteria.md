---
title: Leaderboard Query Filter Criteria
aliases: []
tags:
- concept
summary: 生成 leaderboard 所需查询的具体过滤条件组合，包括按 competition ID 筛选、只接受通过（passed）的结果，以及可选的
  runtime 与 error 过滤。
created: '2026-08-26'
updated: '2026-08-26'
---

# Leaderboard Query Filter Criteria

%% ytkb:def %%
生成 leaderboard 所需查询的具体过滤条件组合，包括按 competition ID 筛选、只接受通过（passed）的结果，以及可选的 runtime 与 error 过滤。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- leaderboard 查询逻辑：先按 competition ID 过滤，再按提交时间排序，只保留 test case result 为通过（passed）的记录，必要时进一步按 runtime 和 error 过滤，并可统计提交（submit）次数。（[33:10](https://youtu.be/QBHTbtWSECg?t=1990)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[leaderboard-as-derived-query]]
%% ytkb:end %%
