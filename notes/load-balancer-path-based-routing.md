---
title: Load Balancer Path-Based Routing
aliases: []
tags:
- concept
summary: 负载均衡器根据请求路径（如 /api/login）将流量分发到对应微服务的能力。
created: '2026-08-26'
updated: '2026-08-26'
---

# Load Balancer Path-Based Routing

%% ytkb:def %%
负载均衡器根据请求路径（如 /api/login）将流量分发到对应微服务的能力。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 当系统拆分为多个微服务后，负载均衡器需要能识别请求路径（如 POST /api/login）并将其路由到正确的微服务（如 auth service），但并非所有负载均衡器都具备这种基于路径的路由能力。（[18:05](https://youtu.be/Qa-7iWxDz1A?t=1085)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[domain-driven-service-decomposition]]
- [[microservices-architecture]]
%% ytkb:end %%
