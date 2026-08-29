---
title: OAuth 2 Authorization Code Flow
aliases: []
tags:
- concept
summary: OAuth 2 典型的授权流程：应用请求访问用户资源时，先跳转到资源方 consent screen 获取用户同意，再通过 authorization
  code 换取 access token。
created: '2026-08-26'
updated: '2026-08-26'
---

# OAuth 2 Authorization Code Flow

%% ytkb:def %%
OAuth 2 典型的授权流程：应用请求访问用户资源时，先跳转到资源方 consent screen 获取用户同意，再通过 authorization code 换取 access token。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- OAuth 2 流程中，用户被重定向到资源方（如 Google）的 consent screen 查看权限请求，一旦用户同意，资源方会向发起请求的应用返回一个 authorization code，随后该应用用这个 code 去交换出真正可用于读取数据的 access token。（[96:26](https://youtu.be/oYxTTirKY8M?t=5786)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[oauth2-authorization-framework]]
%% ytkb:end %%
