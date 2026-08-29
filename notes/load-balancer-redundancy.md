---
title: Load Balancer Redundancy
aliases: []
tags:
- concept
summary: 通过部署多个 load balancer 实例来避免单个 load balancer 成为单点故障的策略。
created: '2026-08-26'
updated: '2026-08-26'
---

# Load Balancer Redundancy

%% ytkb:def %%
通过部署多个 load balancer 实例来避免单个 load balancer 成为单点故障的策略。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 为避免 load balancer 成为单点故障，可部署多个 load balancer：当一个宕机时将全部流量重定向到另一个，待其恢复后再按比例（如50%）重新分配流量。（[27:03](https://youtu.be/oYxTTirKY8M?t=1623)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[load-balancer]]
- [[load-balancer-health-monitoring]]
- [[single-point-of-failure]]
%% ytkb:end %%
