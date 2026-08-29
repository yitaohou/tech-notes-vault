---
title: Weighted Load Balancing Variant
aliases: []
tags:
- concept
summary: 基于服务器容量和性能指标（如RAM大小）为其分配权重、再据权重比例分配流量的负载均衡算法变体，如weighted round robin或weighted
  least connections。
created: '2026-08-26'
updated: '2026-08-26'
---

# Weighted Load Balancing Variant

%% ytkb:def %%
基于服务器容量和性能指标（如RAM大小）为其分配权重、再据权重比例分配流量的负载均衡算法变体，如weighted round robin或weighted least connections。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 加权类负载均衡算法（如 weighted round robin、weighted least connections）会根据服务器的硬件容量指标（例如16GB、32GB、64GB的RAM）为每台服务器分配不同权重，权重更高的服务器会被分配更多比例的流量。（[18:02](https://youtu.be/oYxTTirKY8M?t=1082)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[least-connections-load-balancing]]
- [[weighted-round-robin-load-balancing]]
%% ytkb:end %%
