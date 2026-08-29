---
title: Health Check-Based Load Balancing
aliases: []
tags:
- concept
summary: 负载均衡器通过健康检查了解各服务器实时负载状况，并据此动态决定流量分配的技术。
created: '2026-08-26'
updated: '2026-08-26'
---

# Health Check-Based Load Balancing

%% ytkb:def %%
负载均衡器通过健康检查了解各服务器实时负载状况，并据此动态决定流量分配的技术。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 更智能的 load balancer 会用 health check 持续了解各服务器的真实负载情况，如果某台服务器正在处理耗资源的上传任务而明显更忙，就会把新请求优先发送到状态更好的服务器，而不是机械地轮询。（[09:02](https://youtu.be/Qa-7iWxDz1A?t=542)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 负载均衡器会实时判断各服务器当前的负载状况，将新到达的请求转发给负载最小的服务器。（[15:01](https://youtu.be/oYxTTirKY8M?t=901)）
- 大多数负载均衡器通过持续向所有后端服务器发送健康检查请求，实时掌握每台服务器当前是在线还是离线。（[21:03](https://youtu.be/oYxTTirKY8M?t=1263)）
- 当健康检查探测到某台服务器发生故障（离线）后，负载均衡器会记录该状态，后续新请求不再被路由到这台故障服务器。（[21:03](https://youtu.be/oYxTTirKY8M?t=1263)）
- Nginx 内置健康检查功能，会持续监控各服务器状态，一旦某台服务器宕机就停止向其转发流量。（[24:03](https://youtu.be/oYxTTirKY8M?t=1443)）
- 云托管负载均衡器自带的 monitoring 功能本质上等同于健康检查，无需用户自行搭建。（[24:03](https://youtu.be/oYxTTirKY8M?t=1443)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[consistent-hashing-failover]]
- [[load-balancer]]
- [[load-balancer-traffic-asymmetry]]
- [[managed-load-balancer-provisioning]]
- [[nginx-load-balancer]]
%% ytkb:end %%
