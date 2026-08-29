---
title: HTTP 201 Created
aliases: []
tags:
- concept
summary: 表示请求已成功且服务端新创建了一个资源的 HTTP 状态码。
created: '2026-08-26'
updated: '2026-08-26'
---

# HTTP 201 Created

%% ytkb:def %%
表示请求已成功且服务端新创建了一个资源的 HTTP 状态码。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 创建资源的 POST 请求成功后应返回 201（Created）而非 200，因为 200 只表示笼统成功，201 专门表示新资源已被创建。（[72:17](https://youtu.be/oYxTTirKY8M?t=4337)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[http-200-ok]]
- [[http-status-code-categories]]
%% ytkb:end %%
