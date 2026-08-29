---
title: Cursor-based Pagination
aliases: []
tags:
- concept
summary: 一种分页方式，用一个代表目标数据位置的哈希值（cursor）代替 page 或 offset 与 limit 参数来定位要获取的数据。
created: '2026-08-26'
updated: '2026-08-26'
---

# Cursor-based Pagination

%% ytkb:def %%
一种分页方式，用一个代表目标数据位置的哈希值（cursor）代替 page 或 offset 与 limit 参数来定位要获取的数据。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- cursor-based pagination 用一个 cursor（代表要获取页面位置的哈希值）取代 page 和 limit 参数，是分页实现的第三种常见方案。（[1:06:15](https://youtu.be/oYxTTirKY8M?t=3975)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[offset-based-pagination]]
- [[pagination-api-design]]
%% ytkb:end %%
