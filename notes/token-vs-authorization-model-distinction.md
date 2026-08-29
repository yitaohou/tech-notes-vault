---
title: Token vs Authorization Model Distinction
aliases: []
tags:
- concept
summary: token（如 JWT）只是承载用户身份与声明信息的传输机制，而 role-based、attribute-based 等 authorization
  model 才是真正定义用户被允许访问什么的规则体系。
created: '2026-08-26'
updated: '2026-08-26'
---

# Token vs Authorization Model Distinction

%% ytkb:def %%
token（如 JWT）只是承载用户身份与声明信息的传输机制，而 role-based、attribute-based 等 authorization model 才是真正定义用户被允许访问什么的规则体系。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- token 通常携带用户的身份和声明信息，而 authorization model（如 RBAC、ABAC）才是定义用户可访问内容的规则，二者属于不同层面的概念，不应混淆。（[1:54:33](https://youtu.be/oYxTTirKY8M?t=6873)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authentication-vs-authorization]]
- [[jwt-token-authentication]]
%% ytkb:end %%
