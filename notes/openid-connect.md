---
title: OpenID Connect (OIDC)
aliases: []
tags:
- concept
summary: OpenID Connect 是在 OAuth 2 基础上叠加身份认证层的协议，通过 ID token 让应用获知用户身份。
created: '2026-08-26'
updated: '2026-08-26'
---

# OpenID Connect (OIDC)

%% ytkb:def %%
OpenID Connect 是在 OAuth 2 基础上叠加身份认证层的协议，通过 ID token 让应用获知用户身份。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- OpenID Connect 在 OAuth 2 的授权能力之上增加了认证（authentication）能力，这是二者的核心区别。（[99:28](https://youtu.be/oYxTTirKY8M?t=5968)）
- 点击「通过 Google 登录」会先跳转到 identity provider 的 authorization endpoint 显示登录页，用户输入凭证并同意授权后，provider 会返回一个 authorization code。（[99:28](https://youtu.be/oYxTTirKY8M?t=5968)）
- OIDC 被认为是现代、安全且可扩展的认证方案，这也是「Sign in with Google/GitHub/Microsoft」这类第三方登录普遍采用它的原因。（[99:28](https://youtu.be/oYxTTirKY8M?t=5968)）
- 使用 OpenID Connect 认证时，用户被重定向到登录页面并提供凭证，认证通过后系统返回 JWT 格式的 ID token，用于向应用确认用户身份。（[1:42:29](https://youtu.be/oYxTTirKY8M?t=6149)）
- Google 等公司在底层采用 OpenID Connect 作为身份协议，它比 SAML 更现代，但两者目前都仍是安全且常用的认证方案。（[1:42:29](https://youtu.be/oYxTTirKY8M?t=6149)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[jwt-token-authentication]]
- [[oauth2-access-token]]
- [[oidc-id-token]]
- [[saml]]
- [[single-sign-on]]
%% ytkb:end %%
