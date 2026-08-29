---
title: Refresh Token HTTP-Only Cookie Storage
aliases: []
tags:
- concept
summary: 为防止 XSS 攻击窃取 token，refresh token 不存放在浏览器 local storage 中，而是存放在 HTTP only
  cookie 中的做法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Refresh Token HTTP-Only Cookie Storage

%% ytkb:def %%
为防止 XSS 攻击窃取 token，refresh token 不存放在浏览器 local storage 中，而是存放在 HTTP only cookie 中的做法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-authentication-authorization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- refresh token 绝不应存储在 local storage，而应存储在 HTTP only cookie 中，以避免客户端被 XSS 攻击窃取长期有效的 refresh token。（[96:26](https://youtu.be/oYxTTirKY8M?t=5786)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[access-refresh-token-pattern]]
%% ytkb:end %%
