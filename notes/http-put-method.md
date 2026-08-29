---
title: HTTP PUT Method
aliases: []
tags:
- concept
summary: REST API 中用于整体替换（覆盖）已有资源的 HTTP 方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# HTTP PUT Method

%% ytkb:def %%
REST API 中用于整体替换（覆盖）已有资源的 HTTP 方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- PUT 方法请求路径形如 /products/{id}，会用前端传来的新数据完整替换掉数据库中该 ID 对应的整条资源记录。（[70:45](https://youtu.be/oYxTTirKY8M?t=4245)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[http-patch-method]]
- [[restful-api-design]]
%% ytkb:end %%
