---
title: HTTP POST Method
aliases: []
tags:
- concept
summary: REST API 中用于在服务器创建新资源的 HTTP 方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# HTTP POST Method

%% ytkb:def %%
REST API 中用于在服务器创建新资源的 HTTP 方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- POST 方法请求路径与 GET 相同（如 /products），但语义是创建资源而非检索，对应 CRUD 中的 Create 操作。（[70:10](https://youtu.be/oYxTTirKY8M?t=4210)）
- POST 请求会改变服务器状态且不是幂等的：每次创建资源都会生成一个新的 ID（第一次创建得到 ID 1，第二次得到 ID 2，以此类推）。（[70:25](https://youtu.be/oYxTTirKY8M?t=4225)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[http-get-method]]
- [[http-idempotency]]
- [[restful-api-design]]
%% ytkb:end %%
