---
title: Node.js Server Concurrent Request Capacity
aliases: []
tags:
- concept
summary: 经过良好优化的单个 Node.js 服务器通常能承载的并发请求数量区间。
created: '2026-08-26'
updated: '2026-08-26'
---

# Node.js Server Concurrent Request Capacity

%% ytkb:def %%
经过良好优化的单个 Node.js 服务器通常能承载的并发请求数量区间。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 一台经过良好优化的 Node.js 服务器通常可以支撑 2000 到 10000 个并发请求，超过这个范围就需要考虑扩展方式。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[horizontal-scaling]]
- [[load-balancer]]
%% ytkb:end %%
