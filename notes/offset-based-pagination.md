---
title: Offset-based Pagination
aliases: []
tags:
- concept
summary: 一种分页方式，用 offset 参数指定从数据集的第几项开始计数读取，并结合 limit 限制返回条目数量。
created: '2026-08-26'
updated: '2026-08-26'
---

# Offset-based Pagination

%% ytkb:def %%
一种分页方式，用 offset 参数指定从数据集的第几项开始计数读取，并结合 limit 限制返回条目数量。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 部分 API 用 offset 取代 page 参数实现分页：offset 告诉 API 从数据集的第几项开始计数，再配合 limit 限制本次返回的条目数量。（[1:06:15](https://youtu.be/oYxTTirKY8M?t=3975)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cursor-based-pagination]]
- [[pagination-api-design]]
%% ytkb:end %%
