---
title: HTTP Method Determines Resource Action
aliases: []
tags:
- concept
summary: 在 REST 设计中，同一个资源 URL（如 /orders）具体执行的操作由所使用的 HTTP 方法决定，而非由 URL 本身表达动作。
created: '2026-08-26'
updated: '2026-08-26'
---

# HTTP Method Determines Resource Action

%% ytkb:def %%
在 REST 设计中，同一个资源 URL（如 /orders）具体执行的操作由所使用的 HTTP 方法决定，而非由 URL 本身表达动作。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 同样是 /orders 这个 URL，用 GET 方法请求会返回订单列表，用 POST 方法请求则会创建一个新订单，动作语义完全由 HTTP 方法承担。（[63:13](https://youtu.be/oYxTTirKY8M?t=3793)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rest-noun-based-url-design]]
%% ytkb:end %%
