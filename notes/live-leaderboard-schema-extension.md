---
title: Live Leaderboard via Schema Extension
aliases: []
tags:
- concept
summary: 在已有系统架构基础上，仅通过新增一张记录提交（submission）详情的数据库 schema 即可支持周赛/双周赛实时排行榜功能。
created: '2026-08-26'
updated: '2026-08-26'
---

# Live Leaderboard via Schema Extension

%% ytkb:def %%
在已有系统架构基础上，仅通过新增一张记录提交（submission）详情的数据库 schema 即可支持周赛/双周赛实时排行榜功能。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 对于 lead code 周赛和双周赛的实时排行榜（live leaderboard）需求，现有架构基本可以直接复用，只需新增一张存储提交详情及其关联信息的 schema，无需大改架构。（[30:08](https://youtu.be/QBHTbtWSECg?t=1808)）
%% ytkb:end %%
