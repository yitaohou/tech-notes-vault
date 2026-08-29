---
title: Bearer Token Pattern
aliases: []
tags:
- concept
summary: 一种认证模式：任何持有该 token 的一方都能凭它获得访问权限，本身不是具体的实现方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Bearer Token Pattern

%% ytkb:def %%
一种认证模式：任何持有该 token 的一方都能凭它获得访问权限，本身不是具体的实现方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 开发者常混淆 bearer token 与 JWT：bearer token 只是一种模式（谁拥有该 token 谁就能访问），而 JWT 是 bearer token 最常见的具体实现类型。（[93:24](https://youtu.be/oYxTTirKY8M?t=5604)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[jwt-token-authentication]]
%% ytkb:end %%
