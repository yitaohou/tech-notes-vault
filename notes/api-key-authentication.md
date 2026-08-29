---
title: API Key Authentication
aliases: []
tags:
- concept
summary: API key authentication 是为每个 client 生成唯一 key、并要求其在后续每次请求中携带该 key 以访问资源的认证方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Key Authentication

%% ytkb:def %%
API key authentication 是为每个 client 生成唯一 key、并要求其在后续每次请求中携带该 key 以访问资源的认证方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- API key authentication 中，服务端为每个 client 生成一个唯一的 key，client 之后每次请求都携带该 key（通过 Authorization header 或专门的 X-API-Key header）来访问资源。（[87:22](https://youtu.be/oYxTTirKY8M?t=5242)）
- 生成的 API key 通常会被存储在数据库中，供服务端后续校验客户端请求时使用。（[87:22](https://youtu.be/oYxTTirKY8M?t=5242)）
- 使用 API key 访问服务时，服务器会在 permissions 或 users 表中查找该 key，验证通过则返回带数据的成功响应，验证失败则返回 401 unauthorized。（[90:23](https://youtu.be/oYxTTirKY8M?t=5423)）
- 如果请求中完全缺失 API key（如 authorization header 或 X-API-Key 均未提供），服务器会返回 400 bad request，因为该类系统强制要求携带 API key。（[90:23](https://youtu.be/oYxTTirKY8M?t=5423)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authorization-header-token-transport]]
- [[unauthorized-401-status-code]]
%% ytkb:end %%
