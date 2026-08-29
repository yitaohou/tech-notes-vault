---
title: Single Sign-On (SSO)
aliases: []
tags:
- concept
summary: SSO（单点登录）是一种用户体验模式而非认证方法，允许用户只登录一次身份提供方（identity provider），即可访问该提供方旗下的多个服务。
created: '2026-08-26'
updated: '2026-08-26'
---

# Single Sign-On (SSO)

%% ytkb:def %%
SSO（单点登录）是一种用户体验模式而非认证方法，允许用户只登录一次身份提供方（identity provider），即可访问该提供方旗下的多个服务。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-authentication-authorization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 例如登录 Google 或 Okta 一次后，用户无需再次登录即可访问 Gmail、Google Drive、YouTube、Google Calendar 等多个服务。（[99:28](https://youtu.be/oYxTTirKY8M?t=5968)）
- SSO 底层依赖身份协议（identity protocol）来验证各个服务间共享的会话是否有效。（[99:28](https://youtu.be/oYxTTirKY8M?t=5968)）
- 用户登录 identity provider（如 Google）后，全局会话会被存入 session storage，同时客户端会拿到一个 SSO cookie，凭此 cookie 即可在首次访问 Gmail 等资源时完成会话校验并获得访问权限。（[99:28](https://youtu.be/oYxTTirKY8M?t=5968)）
- SSO 让用户登录一个应用后，其 session 和 cookie 会被复用，访问同一生态下的其他应用（如 Google Drive、YouTube、Google Calendar）时只需验证 session 是否有效，无需重新登录。（[1:42:29](https://youtu.be/oYxTTirKY8M?t=6149)）
- SSO 底层依赖具体的身份协议来实现，主要包括 SAML 和 OpenID Connect 两种协议。（[1:42:29](https://youtu.be/oYxTTirKY8M?t=6149)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[openid-connect]]
- [[saml]]
%% ytkb:end %%
