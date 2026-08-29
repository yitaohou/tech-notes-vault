---
title: Path-Based Load Balancer Routing
aliases: []
tags:
- concept
summary: 负载均衡器根据请求的 API 路径名，将其转发到专门服务的路由能力。
created: '2026-08-26'
updated: '2026-08-26'
---

# Path-Based Load Balancer Routing

%% ytkb:def %%
负载均衡器根据请求的 API 路径名，将其转发到专门服务的路由能力。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-networking]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- load balancer 除了均衡负载外还能基于 API 路径做路由，例如把以上传（POST upload）开头的请求专门转发给负责文件处理的专用服务，让其余服务器只处理常规流量、保持健康状态。（[09:02](https://youtu.be/Qa-7iWxDz1A?t=542)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[health-check-load-balancing]]
- [[load-balancer]]
%% ytkb:end %%
