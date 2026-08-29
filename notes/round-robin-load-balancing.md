---
title: Round Robin Load Balancing
aliases: []
tags:
- concept
summary: 一种轮询式负载均衡算法，按顺序依次把请求分配给不同服务器。
created: '2026-08-26'
updated: '2026-08-26'
---

# Round Robin Load Balancing

%% ytkb:def %%
一种轮询式负载均衡算法，按顺序依次把请求分配给不同服务器。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- round robin 算法让 load balancer 按顺序依次把新请求分配给不同服务器（例如 A 用户到 server 1，下一个用户到 server 2），使各服务器接收到数量相同的请求。（[09:02](https://youtu.be/Qa-7iWxDz1A?t=542)）
- 在 round robin 模式下，客户端每次刷新页面请求会依次命中 server one、server two、server three，循环往复。（[12:03](https://youtu.be/Qa-7iWxDz1A?t=723)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- round robin 是最简单的负载均衡算法：按顺序依次把请求分配给服务器池中的各台服务器，轮到最后一台后再从第一台重新开始循环。（[15:01](https://youtu.be/oYxTTirKY8M?t=901)）
- round robin 算法适用于各服务器硬件规格相近的场景，若服务器性能差异较大则不是好的选择。（[15:01](https://youtu.be/oYxTTirKY8M?t=901)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[least-connections-load-balancing]]
- [[load-balancer]]
- [[nginx-upstream-block]]
- [[sticky-sessions]]
%% ytkb:end %%
