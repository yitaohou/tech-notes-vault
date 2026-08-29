---
title: Access Token / Refresh Token Pattern
aliases: []
tags:
- concept
summary: 现代系统常用的双 token 机制，access token 短生命周期（15分钟到1小时）用于 API 调用鉴权，refresh token 长生命周期（数天到数周）用于在
  access token 过期后换取新的 access token。
created: '2026-08-26'
updated: '2026-08-26'
---

# Access Token / Refresh Token Pattern

%% ytkb:def %%
现代系统常用的双 token 机制，access token 短生命周期（15分钟到1小时）用于 API 调用鉴权，refresh token 长生命周期（数天到数周）用于在 access token 过期后换取新的 access token。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 用户登录成功后会同时拿到 access token 和 refresh token，access token 过期时客户端返回 unauthorized 响应，此时用之前存下的 refresh token 向 auth server 请求新 access token，从而免于让用户重新输入凭证。（[96:26](https://youtu.be/oYxTTirKY8M?t=5786)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authentication-service-login-flow]]
- [[jwt-token-authentication]]
%% ytkb:end %%
