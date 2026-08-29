---
title: HTTP PATCH Method
aliases: []
tags:
- concept
summary: REST API 中用于部分更新已有资源、只修改指定字段而保留其余属性不变的 HTTP 方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# HTTP PATCH Method

%% ytkb:def %%
REST API 中用于部分更新已有资源、只修改指定字段而保留其余属性不变的 HTTP 方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- PATCH 方法与 PUT 使用相同的请求路径（/products/{id}），但只更新请求中提供的部分字段（如仅更新 title），其余属性保持不变。（[71:05](https://youtu.be/oYxTTirKY8M?t=4265)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[http-put-method]]
%% ytkb:end %%
