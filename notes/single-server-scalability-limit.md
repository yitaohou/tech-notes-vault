---
title: Single Server Scalability Limit
aliases: []
tags:
- concept
summary: 单服务器架构在小规模用户下运作良好，但面对大流量时会出现性能瓶颈，是驱动系统架构演进扩展的核心原因。
created: '2026-08-26'
updated: '2026-08-26'
---

# Single Server Scalability Limit

%% ytkb:def %%
单服务器架构在小规模用户下运作良好，但面对大流量时会出现性能瓶颈，是驱动系统架构演进扩展的核心原因。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 单服务器架构适合小规模用户场景，但在高并发或大流量下会难以支撑，这正是后续需要引入横向扩展、负载均衡等手段的原因。（[03:00](https://youtu.be/oYxTTirKY8M?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[horizontal-scaling]]
- [[load-balancer-need-multi-server]]
%% ytkb:end %%
