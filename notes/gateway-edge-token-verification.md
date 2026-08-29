---
title: Gateway Edge Token Verification
aliases: []
tags:
- concept
summary: gateway 在请求到达边缘时就地校验 token 是否有效，无需额外发起网络请求访问认证服务的设计。
created: '2026-08-26'
updated: '2026-08-26'
---

# Gateway Edge Token Verification

%% ytkb:def %%
gateway 在请求到达边缘时就地校验 token 是否有效，无需额外发起网络请求访问认证服务的设计。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- gateway 可以直接在边缘验证请求中携带的 token 是否合法，若合法则信任其未过期，不必对认证服务发起额外的网络调用。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[jwt-token-authentication]]
- [[unauthorized-401-status-code]]
%% ytkb:end %%
