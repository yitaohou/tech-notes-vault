---
title: Leaderboard as a Derived Query
aliases: []
tags:
- concept
summary: leaderboard 不需要单独的数据库 schema，而是通过对已有 submissions 表执行带过滤条件的查询动态生成排行榜结果。
created: '2026-08-26'
updated: '2026-08-26'
---

# Leaderboard as a Derived Query

%% ytkb:def %%
leaderboard 不需要单独的数据库 schema，而是通过对已有 submissions 表执行带过滤条件的查询动态生成排行榜结果。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 设计决策：leaderboard 不需要独立的表 schema，只需在 submissions 表上编写查询（拉取 submitted time、test case result、runtime、error 等字段）即可生成排行榜。（[33:10](https://youtu.be/QBHTbtWSECg?t=1990)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[leaderboard-query-filter-criteria]]
- [[leetcode-submissions-schema]]
%% ytkb:end %%
