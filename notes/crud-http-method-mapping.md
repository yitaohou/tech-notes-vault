---
title: CRUD-to-HTTP Method Mapping
aliases: []
tags:
- concept
summary: REST API 中 Create、Read、Update、Delete 四类操作分别对应 POST、GET、PUT/PATCH、DELETE 这几个
  HTTP 方法的约定。
created: '2026-08-26'
updated: '2026-08-26'
---

# CRUD-to-HTTP Method Mapping

%% ytkb:def %%
REST API 中 Create、Read、Update、Delete 四类操作分别对应 POST、GET、PUT/PATCH、DELETE 这几个 HTTP 方法的约定。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- REST API 依托 HTTP 协议，用 GET/POST/PUT/PATCH/DELETE 这几种 HTTP 方法分别实现读取、创建、更新（整体/部分）、删除这些最常见的 CRUD 操作。（[69:17](https://youtu.be/oYxTTirKY8M?t=4157)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[http-delete-method]]
- [[http-get-method]]
- [[http-patch-method]]
- [[http-post-method]]
- [[http-put-method]]
- [[restful-api-design]]
%% ytkb:end %%
