---
title: Digest Authentication
aliases: []
tags:
- concept
summary: Digest authentication 是一种在请求中发送用户名密码经 MD5 哈希后版本、而非明文的认证方法，流程与 Basic authentication
  类似。
created: '2026-08-26'
updated: '2026-08-26'
---

# Digest Authentication

%% ytkb:def %%
Digest authentication 是一种在请求中发送用户名密码经 MD5 哈希后版本、而非明文的认证方法，流程与 Basic authentication 类似。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-security]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- Digest authentication 的流程与 Basic authentication 类似：先返回 401 unauthorized 提示客户端携带凭证，客户端随后发送包含用户名密码 MD5 哈希值的请求，校验通过则返回用户数据，否则仍返回 401。（[87:22](https://youtu.be/oYxTTirKY8M?t=5242)）
- Digest authentication 因使用 MD5 哈希而比 Basic authentication 略安全，但 MD5 本身已过时，如今在生产环境中也很少被使用。（[87:22](https://youtu.be/oYxTTirKY8M?t=5242)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[basic-authentication]]
- [[unauthorized-401-status-code]]
%% ytkb:end %%
