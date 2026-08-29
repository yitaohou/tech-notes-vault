---
title: Opaque Token (Pre-JWT)
aliases: []
tags:
- concept
summary: 在 JWT 出现之前使用的一种不携带任何信息的纯字符串 token，每次使用都需要在数据库中查找验证。
created: '2026-08-26'
updated: '2026-08-26'
---

# Opaque Token (Pre-JWT)

%% ytkb:def %%
在 JWT 出现之前使用的一种不携带任何信息的纯字符串 token，每次使用都需要在数据库中查找验证。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 在 JWT 出现之前，token 只是一个不携带任何信息的字符串，服务端每次使用时都必须在数据库或缓存中查找该 token 才能验证用户权限，本质上仍是有状态的。（[93:24](https://youtu.be/oYxTTirKY8M?t=5604)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[jwt-token-authentication]]
- [[session-based-authentication]]
%% ytkb:end %%
