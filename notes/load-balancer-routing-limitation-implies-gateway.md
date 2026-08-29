---
title: Load Balancer Routing Limitation Implies Need for Gateway
aliases: []
tags:
- concept
summary: 当负载均衡器无法胜任基于路径的服务路由时，暗示系统可能需要引入专门的网关组件来承担这一职责。
created: '2026-08-26'
updated: '2026-08-26'
---

# Load Balancer Routing Limitation Implies Need for Gateway

%% ytkb:def %%
当负载均衡器无法胜任基于路径的服务路由时，暗示系统可能需要引入专门的网关组件来承担这一职责。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 如果负载均衡器不支持按路径路由到不同微服务，说明负载均衡器可能并不是承担这一路由职责的合适组件，暗示需要额外的路由层（如 API gateway）来解决这个问题。（[18:05](https://youtu.be/Qa-7iWxDz1A?t=1085)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[load-balancer-path-based-routing]]
%% ytkb:end %%
