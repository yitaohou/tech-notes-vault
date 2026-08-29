---
title: Leaderboard API Design
aliases: []
tags:
- concept
summary: 用于获取比赛实时排行榜的 GET API 设计，需要传入 competition ID 作为参数。
created: '2026-08-26'
updated: '2026-08-26'
---

# Leaderboard API Design

%% ytkb:def %%
用于获取比赛实时排行榜的 GET API 设计，需要传入 competition ID 作为参数。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 获取比赛排行榜使用 GET 请求，需要传入 competition ID 作为参数来定位具体比赛的排行数据。（[18:07](https://youtu.be/QBHTbtWSECg?t=1087)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[leaderboard-pagination]]
%% ytkb:end %%
