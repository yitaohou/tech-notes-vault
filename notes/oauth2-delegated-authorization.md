---
title: OAuth 2 Delegated Authorization
aliases: []
tags:
- concept
summary: 一种委托授权协议，用于让某个服务代表用户去访问另一个服务的资源，而无需获取用户的账号密码。
created: '2026-08-26'
updated: '2026-08-26'
---

# OAuth 2 Delegated Authorization

%% ytkb:def %%
一种委托授权协议，用于让某个服务代表用户去访问另一个服务的资源，而无需获取用户的账号密码。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- OAuth 2 是一种委托授权（delegated authorization）协议，当一个服务需要代表用户访问另一服务的资源时使用。（[1:51:32](https://youtu.be/oYxTTirKY8M?t=6692)）
- 典型场景：把 app 部署到 Vercel 时需要让 Vercel 访问你在 GitHub 上的仓库，若直接把 GitHub 用户名密码交给 Vercel 并不安全，因为你无法控制第三方会用这些凭证做什么。（[1:51:32](https://youtu.be/oYxTTirKY8M?t=6692)）
- 在 OAuth 2 流程中，用户以自身身份向第三方应用签署请求以申请访问自己资源的权限，GitHub 等资源方随后签发一个代表用户所批准权限的 access token 给第三方应用，而不是直接暴露密码。（[1:51:32](https://youtu.be/oYxTTirKY8M?t=6692)）
- 用户需要明确指定第三方应用可访问哪些具体资源（如哪些仓库）以及可执行哪些操作（创建、读取、更新或删除），access token 中会携带这些具体权限范围。（[1:51:32](https://youtu.be/oYxTTirKY8M?t=6692)）
- OAuth 2 协议本身定义了安全签发与校验 access token 的标准流程，用户交给第三方应用的是代表其已批准权限的 access token，而非自己的密码。（[1:51:32](https://youtu.be/oYxTTirKY8M?t=6692)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[access-control-list-acl]]
- [[jwt-bearer-token-claims]]
%% ytkb:end %%
