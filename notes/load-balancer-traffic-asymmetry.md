---
title: Load Balancer Traffic Asymmetry
aliases: []
tags:
- concept
summary: 指即使各服务器收到的请求数量相同，不同类型请求消耗的资源也可能完全不同，导致实际负载并不均衡的问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# Load Balancer Traffic Asymmetry

%% ytkb:def %%
指即使各服务器收到的请求数量相同，不同类型请求消耗的资源也可能完全不同，导致实际负载并不均衡的问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- round robin 只保证各服务器收到的请求数量相同，但如果一个用户在上传文件（消耗更多存储和 CPU），另一个用户只是读取文件，两台服务器实际承受的负载其实并不对等。（[09:02](https://youtu.be/Qa-7iWxDz1A?t=542)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[health-check-load-balancing]]
- [[round-robin-load-balancing]]
%% ytkb:end %%
