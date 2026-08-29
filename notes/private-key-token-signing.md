---
title: Private Key Token Signing
aliases: []
tags:
- concept
summary: 认证服务使用私钥对生成的 token 进行签名，以保证其真实性和防篡改。
created: '2026-08-26'
updated: '2026-08-26'
---

# Private Key Token Signing

%% ytkb:def %%
认证服务使用私钥对生成的 token 进行签名，以保证其真实性和防篡改。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-security]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 认证服务使用私钥（private key）对新生成的 token 进行签名，确保该 token 的有效性与可信度。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authentication-service-login-flow]]
- [[jwt-token-authentication]]
%% ytkb:end %%
