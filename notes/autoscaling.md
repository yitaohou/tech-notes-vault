---
title: Autoscaling
aliases: []
tags:
- concept
summary: load balancer 或编排系统根据实时流量自动增减服务器实例数量的机制，例如平时维持最少2个实例，流量高峰时自动扩到10个。
created: '2026-08-26'
updated: '2026-08-26'
---

# Autoscaling

%% ytkb:def %%
load balancer 或编排系统根据实时流量自动增减服务器实例数量的机制，例如平时维持最少2个实例，流量高峰时自动扩到10个。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- autoscaling 允许设定最小实例数（如2个），并在流量增大时自动扩容（如扩到10个），从而在成本与承载能力之间自动平衡。（[16:45](https://youtu.be/Qa-7iWxDz1A?t=1005)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 云托管负载均衡器（如 AWS Elastic Load Balancing）自动内置 autoscaling 能力，能在应用需求增加时自动向服务器池中添加新实例。（[24:03](https://youtu.be/oYxTTirKY8M?t=1443)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[kubernetes-container-orchestration]]
- [[load-balancer]]
- [[managed-load-balancer-provisioning]]
- [[minimum-instance-cost-principle]]
%% ytkb:end %%
