---
title: Leaderboard Database Polling
aliases: []
tags:
- concept
summary: 为获取竞赛排行榜最新数据而周期性直接轮询数据库的简单实现方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Leaderboard Database Polling

%% ytkb:def %%
为获取竞赛排行榜最新数据而周期性直接轮询数据库的简单实现方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 获取竞赛排行榜最直接的做法是周期性轮询数据库（例如每5秒或10秒查询一次），但这种方式会带来较高的数据库负载和较高的延迟，且无法在大量用户同时参赛时良好扩展。（[39:13](https://youtu.be/QBHTbtWSECg?t=2353)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[leaderboard-caching]]
%% ytkb:end %%
