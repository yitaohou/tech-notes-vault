---
title: CSRF Token Defense
aliases: []
tags:
- concept
summary: 在 session cookie 认证基础上额外引入 CSRF token 进行双重校验，用于防御 CSRF 攻击的防御手段。
created: '2026-08-26'
updated: '2026-08-26'
---

# CSRF Token Defense

%% ytkb:def %%
在 session cookie 认证基础上额外引入 CSRF token 进行双重校验，用于防御 CSRF 攻击的防御手段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-security]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 服务端同时校验 session cookie 是否存在、以及请求携带的 CSRF token 是否与服务端记录匹配，只有两者都通过才放行请求，从而拦截来自未知第三方的伪造请求，同时放行用户本人的合法请求。（[2:00:34](https://youtu.be/oYxTTirKY8M?t=7234)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[csrf-attack]]
%% ytkb:end %%
