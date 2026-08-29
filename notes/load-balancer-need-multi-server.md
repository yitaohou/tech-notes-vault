---
title: Need for a Routing Layer With Multiple Servers
aliases: []
tags:
- concept
summary: 当系统扩展到多台服务器实例后，需要在中间引入一个组件来决定每个请求应该路由到哪台服务器，否则各服务器之间虽不必互相通信，但缺乏统一调度会导致问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# Need for a Routing Layer With Multiple Servers

%% ytkb:def %%
当系统扩展到多台服务器实例后，需要在中间引入一个组件来决定每个请求应该路由到哪台服务器，否则各服务器之间虽不必互相通信，但缺乏统一调度会导致问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 把服务器扩展成两个实例后，虽然多个服务器之间不需要相互通信，但仍需要一个中间层来决定某个请求具体交给哪台服务器处理，这是进入分布式架构后新出现的问题。（[06:01](https://youtu.be/Qa-7iWxDz1A?t=361)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 当系统从单台服务器扩展为多台服务器（如三台）后，需要引入一个中间组件来决定每个客户端请求（无论来自mobile app还是desktop）应路由到哪台服务器。（[12:00](https://youtu.be/oYxTTirKY8M?t=720)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[horizontal-scaling]]
- [[load-balancer]]
- [[uneven-load-distribution-degraded-experience]]
%% ytkb:end %%
