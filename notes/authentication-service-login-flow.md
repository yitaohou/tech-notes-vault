---
title: Authentication Service Login Flow
aliases: []
tags:
- concept
summary: 负责处理登录页面提交的凭证（如邮箱密码或单点登录令牌）并签发 token 的后端服务及其工作流程。
created: '2026-08-26'
updated: '2026-08-26'
---

# Authentication Service Login Flow

%% ytkb:def %%
负责处理登录页面提交的凭证（如邮箱密码或单点登录令牌）并签发 token 的后端服务及其工作流程。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-authentication-authorization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 用户在登录页面提交凭证（邮箱密码或 single sign-on token）后，由 gateway 将请求重定向到认证服务，由其验证凭证并签发 token。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 客户端首次提交凭据后，认证服务校验合法性并生成 JWT 返回给客户端；此后客户端的后续请求都在 authorization header 中携带该 bearer token 完成认证。（[93:24](https://youtu.be/oYxTTirKY8M?t=5604)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authorization-header-token-transport]]
- [[jwt-token-authentication]]
- [[private-key-token-signing]]
- [[user-existence-check-before-auth]]
%% ytkb:end %%
