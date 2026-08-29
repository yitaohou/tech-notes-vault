---
title: API Sorting via Query Parameter
aliases: []
tags:
- concept
summary: 通过 query parameter（如 sort=price_asc）让后端完成排序，避免前端为排序而拉取全部数据。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Sorting via Query Parameter

%% ytkb:def %%
通过 query parameter（如 sort=price_asc）让后端完成排序，避免前端为排序而拉取全部数据。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 服务端排序功能通过 query parameter（如 sort 属性，取值可为按价格升序、按评论数升序或降序等）实现，客户端传入该参数即可拿到已排好序的结果。（[1:06:15](https://youtu.be/oYxTTirKY8M?t=3975)）
- 如果不在后端做排序，前端要对例如数据库中1000条记录按价格升序排列，就必须先把全部1000条数据都请求下来，效率非常低，因此排序应放在后端完成。（[1:06:15](https://youtu.be/oYxTTirKY8M?t=3975)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-endpoint-filtering]]
- [[pagination-api-design]]
%% ytkb:end %%
