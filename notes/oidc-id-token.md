---
title: OIDC ID Token
aliases: []
tags:
- concept
summary: ID token 是 OIDC 流程中随 access token 一起返回的 JSON Web Token，携带用户的邮箱、用户名、用户 ID
  等身份信息。
created: '2026-08-26'
updated: '2026-08-26'
---

# OIDC ID Token

%% ytkb:def %%
ID token 是 OIDC 流程中随 access token 一起返回的 JSON Web Token，携带用户的邮箱、用户名、用户 ID 等身份信息。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 应用用 authorization code 换取 token 时会同时拿到 access token 和 ID token：access token 用于 OAuth 2 授权访问资源，ID token 则是包含用户身份的 JWT。（[99:28](https://youtu.be/oYxTTirKY8M?t=5968)）
- 应用拿到 ID token 后会验证其签名、提取出用户身份，再把 ID token 发给自己的后端做校验，随后后端为该用户创建自己的 session 并持有对应的 access token。（[99:28](https://youtu.be/oYxTTirKY8M?t=5968)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[jwt-token-authentication]]
- [[oauth2-access-token]]
- [[openid-connect]]
%% ytkb:end %%
