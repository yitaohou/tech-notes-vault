---
title: Authorization Header Token Transport
aliases: []
tags:
- concept
summary: 客户端通过 HTTP 的 authorization header（或 cookie）将 token 附加在请求中发送给服务端的方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Authorization Header Token Transport

%% ytkb:def %%
客户端通过 HTTP 的 authorization header（或 cookie）将 token 附加在请求中发送给服务端的方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 用户发送请求时把 token 放在 authorization header 中，这也是使用 cookie 传递身份凭证的常见做法。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 客户端请求携带的 authorization header 中包含认证类型（如 bearer）以及具体的 token 值，服务端据此校验该 token。（[93:24](https://youtu.be/oYxTTirKY8M?t=5604)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[bearer-token-pattern]]
- [[jwt-token-authentication]]
%% ytkb:end %%
