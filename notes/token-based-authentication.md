---
title: Token-Based Authentication
aliases: []
tags:
- concept
summary: 现代应用普遍采用的认证范式，客户端在每次请求中携带 token，而非依赖服务端维护的 session 状态。
created: '2026-08-26'
updated: '2026-08-26'
---

# Token-Based Authentication

%% ytkb:def %%
现代应用普遍采用的认证范式，客户端在每次请求中携带 token，而非依赖服务端维护的 session 状态。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-authentication-authorization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 与 session-based authentication 不同，token-based authentication 让客户端在每次请求中附带 token（而非依赖服务器记住会话），是现代应用的主流认证方式。（[93:24](https://youtu.be/oYxTTirKY8M?t=5604)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authorization-header-token-transport]]
- [[jwt-token-authentication]]
- [[session-based-authentication]]
%% ytkb:end %%
