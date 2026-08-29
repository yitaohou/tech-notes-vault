---
title: Eventual Consistency Example (Problem Count Variance)
aliases: []
tags:
- concept
summary: 用不同用户在同一时刻看到的题目总数可以存在小幅偏差（如相差约10道）来具体化系统可接受的 eventual consistency 范围的例子。
created: '2026-08-26'
updated: '2026-08-26'
---

# Eventual Consistency Example (Problem Count Variance)

%% ytkb:def %%
用不同用户在同一时刻看到的题目总数可以存在小幅偏差（如相差约10道）来具体化系统可接受的 eventual consistency 范围的例子。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 在 LeetCode 系统设计中，不同用户在同一时刻看到的题目列表数量可以有小幅偏差（例如相差约10道），这种偏差属于可接受的 eventual consistency 范围，比服务不可用要好得多。（[03:01](https://youtu.be/QBHTbtWSECg?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[availability-over-consistency-tradeoff]]
%% ytkb:end %%
