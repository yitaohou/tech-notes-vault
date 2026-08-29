---
title: Geographic (Location-Based) Load Balancing
aliases: []
tags:
- concept
summary: 根据用户的地理位置（通常通过IP地址判断）将请求路由到地理上最近的服务器的负载均衡算法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Geographic (Location-Based) Load Balancing

%% ytkb:def %%
根据用户的地理位置（通常通过IP地址判断）将请求路由到地理上最近的服务器的负载均衡算法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 地理位置负载均衡会为不同地区（如 US East、US West、Europe）分别部署服务器，并根据请求方 IP 所在地域将其导向地理上最近的服务器节点。（[21:03](https://youtu.be/oYxTTirKY8M?t=1263)）
- 地理位置负载均衡尤其适用于对延迟敏感的全球化服务场景，因为可以让请求就近由最接近用户的节点处理。（[21:03](https://youtu.be/oYxTTirKY8M?t=1263)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cdn-latency-improvement-example]]
- [[cdn-point-of-presence]]
- [[load-balancer]]
%% ytkb:end %%
