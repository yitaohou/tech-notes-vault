---
title: HTTP Idempotency
aliases: []
tags:
- concept
summary: 指对同一资源重复发起相同请求会得到相同结果、不会产生额外副作用的 HTTP 请求属性。
created: '2026-08-26'
updated: '2026-08-26'
---

# HTTP Idempotency

%% ytkb:def %%
指对同一资源重复发起相同请求会得到相同结果、不会产生额外副作用的 HTTP 请求属性。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- GET 请求既是安全的又是幂等的（idempotent），意味着多次请求 /products 在数据库无变化时会返回完全相同的结果。（[69:40](https://youtu.be/oYxTTirKY8M?t=4180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[http-get-method]]
- [[http-post-method]]
%% ytkb:end %%
