---
title: Self-Healing System
aliases: []
tags:
- concept
summary: 持续监控组件健康状态，一旦检测到故障就自动用同一实例的全新副本替换该组件，从而避免服务中断的机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# Self-Healing System

%% ytkb:def %%
持续监控组件健康状态，一旦检测到故障就自动用同一实例的全新副本替换该组件，从而避免服务中断的机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 自愈系统会持续监控 load balancer 等组件的健康状态，一旦发现其宕机，就自动启动一个同类型的新实例替换它，从而不中断客户端连接。（[27:03](https://youtu.be/oYxTTirKY8M?t=1623)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[autoscaling]]
- [[load-balancer-health-monitoring]]
%% ytkb:end %%
