---
title: Load Balancer
aliases: []
tags:
- concept
summary: 位于客户端与多台服务器之间的中间层组件，负责把请求转发到健康的服务器实例。
created: '2026-08-26'
updated: '2026-08-26'
---

# Load Balancer

%% ytkb:def %%
位于客户端与多台服务器之间的中间层组件，负责把请求转发到健康的服务器实例。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- load balancer 是架构中位于服务器前方的中间层组件，作用是把用户请求转发给一台健康的服务器，而不是让用户直接访问某台固定服务器。（[09:02](https://youtu.be/Qa-7iWxDz1A?t=542)）
- 有了 load balancer 之后，系统理论上可以拥有任意数量的服务器，唯一的限制是能否负担相应的费用。（[15:03](https://youtu.be/Qa-7iWxDz1A?t=903)）
- 为避免 Gateway 自身成为单点故障，可以在 Gateway 前方再部署一层负载均衡器。（[21:05](https://youtu.be/Qa-7iWxDz1A?t=1265)）
- 集群内部的负载均衡器还能帮助判断哪些后端服务需要更多资源，从而指导对该服务的扩容决策。（[21:05](https://youtu.be/Qa-7iWxDz1A?t=1265)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 当单台服务器的并发处理能力达到上限时，最简单的扩展方式是创建多个相同的服务器实例，并引入一个应用负载均衡器（application load balancer）在这些实例之间分配流量。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
- 负载均衡本身是一个独立的大话题，存在多种流量分配方式和判断标准（criteria），前端工程师不需要深入掌握细节，但应该知道其存在并能大致讲清楚原理。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-gateway]]
- [[autoscaling]]
- [[horizontal-scaling]]
- [[nodejs-server-capacity]]
- [[single-point-of-failure]]
- [[vertical-scaling]]
%% ytkb:end %%
