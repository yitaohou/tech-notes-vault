---
title: Consistent Hashing for Failover
aliases:
- Consistent Hashing
tags:
- concept
summary: consistent hashing 是一种在分布式系统中分配请求到节点的技术，当某个节点宕机时可以让其余存活节点继续接管流量。
created: '2026-08-26'
updated: '2026-08-26'
---

# Consistent Hashing for Failover

%% ytkb:def %%
consistent hashing 是一种在分布式系统中分配请求到节点的技术，当某个节点宕机时可以让其余存活节点继续接管流量。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 在多节点分布式架构中使用 consistent hashing，当某个节点宕机时，其余存活节点仍能继续承接流量。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- consistent hashing 使用哈希函数把各台服务器以及基于用户 IP 生成的请求映射到一个环形哈希空间（hash ring）上，请求会被路由到哈希环上离其映射点最近的服务器。（[21:03](https://youtu.be/oYxTTirKY8M?t=1263)）
- consistent hashing 与 IP hashing 类似，能保证同一个客户端的请求持续被路由到同一台服务器上。（[21:03](https://youtu.be/oYxTTirKY8M?t=1263)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[distributed-architecture-avoid-spof]]
- [[load-balancer]]
%% ytkb:end %%
