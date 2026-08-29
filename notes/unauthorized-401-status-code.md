---
title: 401 Unauthorized Status Code
aliases: []
tags:
- concept
summary: 当请求的 token 验证不通过时，在边缘直接返回的 HTTP 401 状态码，表示未授权。
created: '2026-08-26'
updated: '2026-08-26'
---

# 401 Unauthorized Status Code

%% ytkb:def %%
当请求的 token 验证不通过时，在边缘直接返回的 HTTP 401 状态码，表示未授权。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 若 gateway 边缘验证发现 token 无效，会直接抛出 401 状态码拒绝该请求，而不必转发到后端服务。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- HTTP 401 属于 4xx 客户端错误系列，表示用户未通过身份验证、无权发起该请求。（[72:17](https://youtu.be/oYxTTirKY8M?t=4337)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[gateway-edge-token-verification]]
- [[http-400-bad-request]]
- [[http-status-code-categories]]
%% ytkb:end %%
