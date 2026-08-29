---
title: Load Balancer Fault Tolerance
aliases: []
tags:
- concept
summary: 负载均衡器检测到某台服务器宕机后自动停止向其转发流量、并把流量转移给其余可用服务器，待该服务器恢复后再重新纳入分配的容错机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# Load Balancer Fault Tolerance

%% ytkb:def %%
负载均衡器检测到某台服务器宕机后自动停止向其转发流量、并把流量转移给其余可用服务器，待该服务器恢复后再重新纳入分配的容错机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 当某台服务器（如 server 3）宕机时，负载均衡器会停止向其发送流量，把所有请求转移给剩余可用的服务器，直到该服务器重新恢复可用。（[15:01](https://youtu.be/oYxTTirKY8M?t=901)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[fault-tolerance-requirement]]
- [[load-balancer]]
- [[single-point-of-failure]]
%% ytkb:end %%
