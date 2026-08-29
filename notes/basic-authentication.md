---
title: Basic Authentication
aliases: []
tags:
- concept
summary: HTTP Basic Authentication 是把用户名密码进行 base64 编码后随每次请求发送给服务器进行校验的认证方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Basic Authentication

%% ytkb:def %%
HTTP Basic Authentication 是把用户名密码进行 base64 编码后随每次请求发送给服务器进行校验的认证方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- Basic authentication 的流程是服务端在凭证校验通过后返回 200 OK 及用户数据，校验失败则返回 401 unauthorized。（[87:22](https://youtu.be/oYxTTirKY8M?t=5242)）
- base64 编码容易被逆向还原，因此 Basic authentication 若不搭配 HTTPS 使用就不安全；即便配合 HTTPS，由于每次请求都要携带凭证，如今在生产环境中也很少使用，通常只用于内部工具。（[87:22](https://youtu.be/oYxTTirKY8M?t=5242)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-gateway-https-http-boundary]]
- [[digest-authentication]]
- [[unauthorized-401-status-code]]
%% ytkb:end %%
