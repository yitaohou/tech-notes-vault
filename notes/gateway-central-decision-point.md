---
title: Gateway as Central Decision Point
aliases: []
tags:
- concept
summary: 在后端架构中，gateway 作为请求处理链路的中间层，承担认证校验、路由转发等关键决策职责的角色定位。
created: '2026-08-26'
updated: '2026-08-26'
---

# Gateway as Central Decision Point

%% ytkb:def %%
在后端架构中，gateway 作为请求处理链路的中间层，承担认证校验、路由转发等关键决策职责的角色定位。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- gateway 在整个架构中扮演居中决策者的角色，例如决定请求是否需要转发到认证服务、是否需要在边缘直接拒绝请求等。（[24:05](https://youtu.be/Qa-7iWxDz1A?t=1445)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authentication-service-login-flow]]
- [[gateway-edge-token-verification]]
%% ytkb:end %%
