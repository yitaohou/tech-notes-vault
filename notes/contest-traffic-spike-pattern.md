---
title: Contest Traffic Spike Pattern
aliases: []
tags:
- concept
summary: 在类似 LeetCode 的系统中，比赛（contest）期间并发用户数会远高于平时，因为大量用户会在同一时间窗口访问同一批题目。
created: '2026-08-26'
updated: '2026-08-26'
---

# Contest Traffic Spike Pattern

%% ytkb:def %%
在类似 LeetCode 的系统中，比赛（contest）期间并发用户数会远高于平时，因为大量用户会在同一时间窗口访问同一批题目。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 设计可扩展性需求时要注意，比赛期间的并发用户量（QPS）会远高于非比赛时段，属于突发流量场景。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dau-mau-scale-requirement]]
- [[passive-vs-contest-usage-pattern]]
%% ytkb:end %%
