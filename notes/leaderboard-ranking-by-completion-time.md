---
title: Leaderboard Ranking by Completion Time
aliases: []
tags:
- concept
summary: leaderboard 的排名逻辑：用户完成提交的速度越快，其在榜单上的排名越靠前。
created: '2026-08-26'
updated: '2026-08-26'
---

# Leaderboard Ranking by Completion Time

%% ytkb:def %%
leaderboard 的排名逻辑：用户完成提交的速度越快，其在榜单上的排名越靠前。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- submissions 表中记录时间戳（timestamp）的原因是排行榜排名规则依据完成速度：越快完成得分越高的排名。（[33:10](https://youtu.be/QBHTbtWSECg?t=1990)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[leetcode-submissions-schema]]
%% ytkb:end %%
