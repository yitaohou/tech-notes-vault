---
title: Partition Key as Index for Faster Lookup
aliases: []
tags:
- concept
summary: 把某个字段设为 partition key 相当于在该字段上建立索引，从而加快按该字段进行的查询速度。
created: '2026-08-26'
updated: '2026-08-26'
---

# Partition Key as Index for Faster Lookup

%% ytkb:def %%
把某个字段设为 partition key 相当于在该字段上建立索引，从而加快按该字段进行的查询速度。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-data-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 把 competition ID 设为 submissions 表的 partition key，本质上是在该字段上建立索引，使得按特定 competition 拉取全部提交记录的查询速度更快。（[33:10](https://youtu.be/QBHTbtWSECg?t=1990)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[partition-key-selection-by-query-pattern]]
%% ytkb:end %%
