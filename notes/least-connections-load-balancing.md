---
title: Least Connections Load Balancing
aliases: []
tags:
- concept
summary: 一种负载均衡算法，优先把新请求分配给当前活跃连接数最少的服务器，以为最空闲的服务器分配更多流量。
created: '2026-08-26'
updated: '2026-08-26'
---

# Least Connections Load Balancing

%% ytkb:def %%
一种负载均衡算法，优先把新请求分配给当前活跃连接数最少的服务器，以为最空闲的服务器分配更多流量。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- least connections 算法的逻辑是：如果某台服务器当前连接数更少，说明它更空闲、可用性更高，因此优先把新请求路由给它。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- least connections 算法把新请求导向当前活跃连接数最少的服务器；例如三台服务器分别有10、9、30个活跃连接时，新请求会被导向活跃连接数为9的那台服务器。（[15:01](https://youtu.be/oYxTTirKY8M?t=901)）
- least connections 算法特别适合会话时长差异很大的应用场景（比如有的会话持续10分钟、有的只持续1分钟），因为它会把新请求发送给当前活跃连接数最少的服务器。（[18:02](https://youtu.be/oYxTTirKY8M?t=1082)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[load-balancer]]
- [[round-robin-load-balancing]]
%% ytkb:end %%
