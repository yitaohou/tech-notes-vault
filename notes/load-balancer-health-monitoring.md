---
title: Load Balancer Health Monitoring
aliases: []
tags:
- concept
summary: 对 load balancer 自身持续进行健康检查，一旦检测到其宕机就停止向其转发流量，与 load balancer 对后端服务器做健康检查的思路相同。
created: '2026-08-26'
updated: '2026-08-26'
---

# Load Balancer Health Monitoring

%% ytkb:def %%
对 load balancer 自身持续进行健康检查，一旦检测到其宕机就停止向其转发流量，与 load balancer 对后端服务器做健康检查的思路相同。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 可以像 load balancer 对服务器做健康检查一样，对 load balancer 自身持续做健康检查，一旦检测到某个 load balancer 宕机，就不再向其转发流量，直至其恢复在线。（[27:03](https://youtu.be/oYxTTirKY8M?t=1623)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[health-check-load-balancing]]
- [[load-balancer-redundancy]]
%% ytkb:end %%
