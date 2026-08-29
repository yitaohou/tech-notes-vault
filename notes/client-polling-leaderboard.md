---
title: Client-Side Polling for Leaderboard Updates
aliases: []
tags:
- concept
summary: 客户端按固定周期主动重新请求最新数据，而非依赖服务端推送更新的机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# Client-Side Polling for Leaderboard Updates

%% ytkb:def %%
客户端按固定周期主动重新请求最新数据，而非依赖服务端推送更新的机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 客户端可以根据比赛的持续时长，周期性地重新拉取（refetch）排行榜数据，以此实现近似实时的更新效果。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[leaderboard-query-flow]]
%% ytkb:end %%
