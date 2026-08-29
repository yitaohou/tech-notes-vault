---
title: Least Response Time Load Balancing
aliases: []
tags:
- concept
summary: 一种同时考虑服务器响应速度与当前活跃连接数、优先将请求发送给响应最快且负载较低服务器的负载均衡算法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Least Response Time Load Balancing

%% ytkb:def %%
一种同时考虑服务器响应速度与当前活跃连接数、优先将请求发送给响应最快且负载较低服务器的负载均衡算法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- least response time 算法会优先把流量导向响应速度最快的服务器，但当该服务器的活跃连接数达到某个阈值（如40个）后，会切换到响应速度次之的服务器分担部分流量（如20个请求），实现响应速度与负载的动态平衡。（[18:02](https://youtu.be/oYxTTirKY8M?t=1082)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[least-connections-load-balancing]]
- [[round-robin-load-balancing]]
%% ytkb:end %%
