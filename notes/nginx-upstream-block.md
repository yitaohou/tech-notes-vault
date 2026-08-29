---
title: Nginx Upstream Block
aliases: []
tags:
- concept
summary: Nginx 配置中用于定义一组后端服务器（upstream）并指定其负载均衡方式的配置块。
created: '2026-08-26'
updated: '2026-08-26'
---

# Nginx Upstream Block

%% ytkb:def %%
Nginx 配置中用于定义一组后端服务器（upstream）并指定其负载均衡方式的配置块。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 该 demo 中 Nginx 配置了两个 upstream block，分别代表两组服务器，使同一个 Nginx 反向代理能够根据请求 URL 路径（如 /rr 对应 round robin，/sticky 对应 session affinity）采用不同的负载均衡策略。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[round-robin-load-balancing]]
- [[sticky-sessions]]
%% ytkb:end %%
