---
title: Gateway as Single Entry Point
aliases: []
tags:
- concept
summary: API Gateway 作为客户端与整个系统通信的唯一入口，统一处理认证与路由的设计。
created: '2026-08-26'
updated: '2026-08-26'
---

# Gateway as Single Entry Point

%% ytkb:def %%
API Gateway 作为客户端与整个系统通信的唯一入口，统一处理认证与路由的设计。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 客户端与业务系统通信的唯一方式是经过 Gateway，Gateway 统一负责处理认证（authentication）和路由（routing）。（[21:05](https://youtu.be/Qa-7iWxDz1A?t=1265)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-gateway]]
- [[vpc-private-network-isolation]]
%% ytkb:end %%
