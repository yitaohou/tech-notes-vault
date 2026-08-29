---
title: Weighted Round Robin Load Balancing
aliases: []
tags:
- concept
summary: round robin 的变体，为每台服务器设置权重，权重越高被分配到的请求比例越大。
created: '2026-08-26'
updated: '2026-08-26'
---

# Weighted Round Robin Load Balancing

%% ytkb:def %%
round robin 的变体，为每台服务器设置权重，权重越高被分配到的请求比例越大。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- weighted round robin 是对基础 round robin 算法的扩展，通过权重让不同服务器承担不同比例的流量。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 在 weighted round robin 算法中，权重更高（性能更强）的服务器会被分配更多连接，权重较低的服务器只接收较小比例的流量。（[21:03](https://youtu.be/oYxTTirKY8M?t=1263)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[load-balancer]]
- [[round-robin-load-balancing]]
%% ytkb:end %%
