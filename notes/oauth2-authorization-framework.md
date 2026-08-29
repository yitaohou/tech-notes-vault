---
title: OAuth 2 as Authorization Framework
aliases: []
tags:
- concept
summary: OAuth 2 是一个常被误解为认证手段的授权框架，回答的是「这个应用可以代表用户访问什么资源」，而非「用户是谁」的认证问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# OAuth 2 as Authorization Framework

%% ytkb:def %%
OAuth 2 是一个常被误解为认证手段的授权框架，回答的是「这个应用可以代表用户访问什么资源」，而非「用户是谁」的认证问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- OAuth 2 本质上是 authorization framework 而非 authentication 方法，用于授权第三方应用代表用户访问指定资源（如 Google Drive 中的文件），而不负责验证用户身份。（[96:26](https://youtu.be/oYxTTirKY8M?t=5786)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authentication-vs-authorization]]
%% ytkb:end %%
