---
title: Pagination Decision Heuristic
aliases: []
tags:
- concept
summary: 判断列表类接口是否需要引入分页的经验法则：数据总量达到数千量级时才有必要分页，数量很少（如几百条）时可不使用。
created: '2026-08-26'
updated: '2026-08-26'
---

# Pagination Decision Heuristic

%% ytkb:def %%
判断列表类接口是否需要引入分页的经验法则：数据总量达到数千量级时才有必要分页，数量很少（如几百条）时可不使用。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 面试者认为若题目总数在几百的量级（如 200 条）可以不用分页，但当数量达到数千量级时始终应该使用分页以避免所有内容显示在同一页面。（[14:20](https://youtu.be/QBHTbtWSECg?t=860)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[pagination-api-design]]
%% ytkb:end %%
