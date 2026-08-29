---
title: SAML (Security Assertion Markup Language)
aliases: []
tags:
- concept
summary: 一种基于 XML 的身份认证协议，常与 SSO 配合使用，多见于企业和 legacy 系统。
created: '2026-08-26'
updated: '2026-08-26'
---

# SAML (Security Assertion Markup Language)

%% ytkb:def %%
一种基于 XML 的身份认证协议，常与 SSO 配合使用，多见于企业和 legacy 系统。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-authentication-authorization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- SAML 是一种基于 XML 的身份协议，常用于 Salesforce、企业仪表盘等 enterprise 和 legacy 系统中的认证场景。（[1:42:29](https://youtu.be/oYxTTirKY8M?t=6149)）
- 使用 SAML 认证时，用户会被重定向到登录页面完成登录，登录成功后系统返回 XML 格式的 SAML assertion 用于确认用户身份，随后即可访问对应的第三方应用。（[1:42:29](https://youtu.be/oYxTTirKY8M?t=6149)）
- 相比 OpenID Connect，SAML 是较旧的身份协议，但目前仍被广泛使用。（[1:42:29](https://youtu.be/oYxTTirKY8M?t=6149)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[openid-connect]]
- [[single-sign-on]]
%% ytkb:end %%
