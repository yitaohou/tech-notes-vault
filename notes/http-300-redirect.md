---
title: HTTP 300 Series Redirection
aliases: []
tags:
- concept
summary: 3xx 系列 HTTP 状态码，用于告知客户端请求的资源已迁移到新地址。
created: '2026-08-26'
updated: '2026-08-26'
---

# HTTP 300 Series Redirection

%% ytkb:def %%
3xx 系列 HTTP 状态码，用于告知客户端请求的资源已迁移到新地址。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 当请求的 URL 对应资源已经迁移到别处时，服务器返回 300 系列状态码并把客户端重定向到新 URL。（[72:17](https://youtu.be/oYxTTirKY8M?t=4337)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[http-status-code-categories]]
%% ytkb:end %%
