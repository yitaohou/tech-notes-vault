---
title: Live Leaderboard Query Flow
aliases: []
tags:
- concept
summary: 实时排行榜功能从客户端请求到返回结果的端到端处理流程。
created: '2026-08-26'
updated: '2026-08-26'
---

# Live Leaderboard Query Flow

%% ytkb:def %%
实时排行榜功能从客户端请求到返回结果的端到端处理流程。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 实时排行榜的端到端流程是：客户端针对某个 competition ID 查询排行榜，后端聚合该比赛下的所有提交并按用户排名，再将排行榜结果返回给客户端。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[client-polling-leaderboard]]
- [[single-api-consolidation]]
%% ytkb:end %%
