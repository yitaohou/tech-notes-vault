---
title: HTTP 404 Not Found
aliases: []
tags:
- concept
summary: 表示客户端请求的具体资源不存在的 HTTP 状态码。
created: '2026-08-26'
updated: '2026-08-26'
---

# HTTP 404 Not Found

%% ytkb:def %%
表示客户端请求的具体资源不存在的 HTTP 状态码。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 当客户端按 ID 查询某个资源（如某个 product）但数据库中不存在该记录时，应返回 404 状态码表示未找到该资源。（[72:17](https://youtu.be/oYxTTirKY8M?t=4337)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[http-400-bad-request]]
- [[http-status-code-categories]]
%% ytkb:end %%
