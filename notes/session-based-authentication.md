---
title: Session-Based Authentication
aliases: []
tags:
- concept
summary: 传统 web 认证方式：用户用凭证登录后，服务器在 session storage 中创建会话，后续请求携带 session cookie 来证明身份。
created: '2026-08-26'
updated: '2026-08-26'
---

# Session-Based Authentication

%% ytkb:def %%
传统 web 认证方式：用户用凭证登录后，服务器在 session storage 中创建会话，后续请求携带 session cookie 来证明身份。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-authentication-authorization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- session-based authentication 的典型流程是：用户登录后服务器生成 session ID 并通过 cookie 下发给客户端，后续请求携带该 cookie 时服务器会在 session storage 中查找会话，找到则视为已认证并返回用户数据，找不到则返回 unauthorized。（[90:23](https://youtu.be/oYxTTirKY8M?t=5423)）
- session-based authentication 是有状态的（stateful），服务器必须用 session storage 记住会话，这种方式适合传统 web 应用，但难以在 API 或分布式系统中扩展。（[93:24](https://youtu.be/oYxTTirKY8M?t=5604)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[jwt-token-authentication]]
- [[session-storage-options]]
- [[token-based-authentication]]
%% ytkb:end %%
