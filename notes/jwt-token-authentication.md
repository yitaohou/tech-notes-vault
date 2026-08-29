---
title: JWT Token Authentication
aliases: []
tags:
- concept
summary: 一种携带签名和过期时间、用于证明用户已通过身份验证的令牌（token）机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# JWT Token Authentication

%% ytkb:def %%
一种携带签名和过期时间、用于证明用户已通过身份验证的令牌（token）机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- JWT token 本质上是一个签名，携带过期时间（expiry date），用来证明请求方已通过身份验证。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- JWT 本质上是一个经过签名的 JSON 对象，其中包含用户 ID 或邮箱等用于验证身份的信息，以及过期时间和角色、权限等其他自定义 claims。（[93:24](https://youtu.be/oYxTTirKY8M?t=5604)）
- JWT 通过签名机制对自身携带的 claims 进行编码和验证，因此可以签发无需查询数据库的短期无状态 token，从而降低数据库负载并简化服务端认证流程。（[93:24](https://youtu.be/oYxTTirKY8M?t=5604)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[bearer-token-pattern]]
- [[gateway-edge-token-verification]]
- [[opaque-token-pre-jwt]]
- [[private-key-token-signing]]
%% ytkb:end %%
