---
title: Single Point of Failure
aliases: []
tags:
- concept
summary: 单点故障指如果所有请求都被路由到同一台服务器，一旦该服务器宕机，所有请求都无法得到响应的情形。
created: '2026-08-26'
updated: '2026-08-26'
---

# Single Point of Failure

%% ytkb:def %%
单点故障指如果所有请求都被路由到同一台服务器，一旦该服务器宕机，所有请求都无法得到响应的情形。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 如果所有查询都被路由到某一台特定服务器，一旦该服务器宕机，就会导致所有查询都无法返回结果，这就是单点故障。（[09:03](https://youtu.be/QBHTbtWSECg?t=543)）
%% ytkb:end %%

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 在只有单一服务器实例、且数据与逻辑都耦合其中的最初架构里，服务器宕机会导致服务不可用与数据丢失双重后果。（[03:00](https://youtu.be/Qa-7iWxDz1A?t=180)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 仅依赖vertical scaling的单台服务器若宕机，将没有其他服务器可用，导致整个应用随之下线，这正是单点故障（single point of failure）风险的体现。（[12:00](https://youtu.be/oYxTTirKY8M?t=720)）
- 单点故障（如数据库或 load balancer）一旦失效会导致整个系统不可用，用户无法访问平台或 checkout 等关键页面，进而造成业务损失。（[27:03](https://youtu.be/oYxTTirKY8M?t=1623)）
- 单点故障（single point of failure）广义上指系统中任意一个组件一旦失效，就会导致整个系统随之无法正常运作。（[24:03](https://youtu.be/oYxTTirKY8M?t=1443)）
- 在客户端经负载均衡器分发请求到多个 API 服务器、但所有服务器共用同一个数据库的架构中，该数据库就是一个单点故障：数据库宕机会导致所有 API 服务器都无法连接数据库，进而使客户端无法收到任何响应。（[24:03](https://youtu.be/oYxTTirKY8M?t=1443)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[database-unsuitable-for-large-files]]
- [[distributed-architecture-avoid-spof]]
- [[fault-tolerance-requirement]]
- [[load-balancer]]
- [[load-balancer-redundancy]]
- [[spof-scalability-risk]]
- [[spof-security-risk]]
- [[stateful-server-data-coupling]]
- [[vertical-scaling]]
%% ytkb:end %%
