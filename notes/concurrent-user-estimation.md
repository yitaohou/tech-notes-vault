---
title: Concurrent User Estimation for Contest
aliases: []
tags:
- concept
summary: 针对特定高峰场景（如竞赛期间）估算并发活跃用户数量的做法，用以区分整体日活/月活与短时高峰负载。
created: '2026-08-26'
updated: '2026-08-26'
---

# Concurrent User Estimation for Contest

%% ytkb:def %%
针对特定高峰场景（如竞赛期间）估算并发活跃用户数量的做法，用以区分整体日活/月活与短时高峰负载。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 系统整体的月活或日活用户可能达到数亿级别，但针对 LeetCode contest 这一具体场景，并发用户量级可估算为 5 万到 10 万左右。（[06:02](https://youtu.be/QBHTbtWSECg?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[contest-traffic-surge]]
- [[scalability-requirement-user-count]]
%% ytkb:end %%
