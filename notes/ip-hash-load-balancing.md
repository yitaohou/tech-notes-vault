---
title: IP Hash Load Balancing
aliases: []
tags:
- concept
summary: 根据客户端IP地址计算哈希值来决定请求应路由到哪台服务器的负载均衡算法，可保证同一客户端始终连接同一服务器。
created: '2026-08-26'
updated: '2026-08-26'
---

# IP Hash Load Balancing

%% ytkb:def %%
根据客户端IP地址计算哈希值来决定请求应路由到哪台服务器的负载均衡算法，可保证同一客户端始终连接同一服务器。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- IP hash 算法通过对客户端的IP地址取哈希值来决定路由目标服务器，从而保证该客户端后续所有请求都被稳定路由到同一台服务器。（[18:02](https://youtu.be/oYxTTirKY8M?t=1082)）
- 当每台服务器都保存了与其所连接客户端相关的信息时，IP hash 是更合适的负载均衡选择，因为它能保证该客户端的请求始终被路由到持有其信息的同一台服务器。（[18:02](https://youtu.be/oYxTTirKY8M?t=1082)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[sticky-sessions]]
%% ytkb:end %%
