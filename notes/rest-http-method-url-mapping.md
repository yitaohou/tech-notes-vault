---
title: REST HTTP Method to URL Mapping
aliases: []
tags:
- concept
summary: REST CRUD 操作要求使用与操作语义匹配的 HTTP 方法搭配资源化 URL，而不是用动作词构造 URL。
created: '2026-08-26'
updated: '2026-08-26'
---

# REST HTTP Method to URL Mapping

%% ytkb:def %%
REST CRUD 操作要求使用与操作语义匹配的 HTTP 方法搭配资源化 URL，而不是用动作词构造 URL。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 删除资源应使用 DELETE 方法请求 /users/{id}，而不应使用 POST 请求 /users/{id} 或类似 /delete 这样的动作式 URL，HTTP 方法和 URL 结构都必须正确设置。（[75:30](https://youtu.be/oYxTTirKY8M?t=4530)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[restful-api-design]]
%% ytkb:end %%
