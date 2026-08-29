---
title: Competition Submission Filtering
aliases: []
tags:
- concept
summary: 在设计比赛排行榜系统时，过滤掉与该 competition 无关的提交（如非参赛的练习提交）的数据处理原则。
created: '2026-08-26'
updated: '2026-08-26'
---

# Competition Submission Filtering

%% ytkb:def %%
在设计比赛排行榜系统时，过滤掉与该 competition 无关的提交（如非参赛的练习提交）的数据处理原则。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 如果用户不是在参加比赛、只是单纯练习刷题，即使他解题速度比所有参赛者都快，这条提交记录对该 competition 的排行榜也是冗余信息，因为根本用不到它，应当被过滤掉。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[leaderboard-query-flow]]
- [[submission-table-user-id]]
%% ytkb:end %%
