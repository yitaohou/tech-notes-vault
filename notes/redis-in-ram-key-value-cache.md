---
title: Redis In-RAM Key-Value Cache
aliases: []
tags:
- concept
summary: Redis 是一种基于 RAM 的 key-value 存储，常用作缓存层，因为从 RAM 读取数据比从磁盘读取快得多。
created: '2026-08-26'
updated: '2026-08-26'
---

# Redis In-RAM Key-Value Cache

%% ytkb:def %%
Redis 是一种基于 RAM 的 key-value 存储，常用作缓存层，因为从 RAM 读取数据比从磁盘读取快得多。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- Redis 是一种 key-value storage，把值缓存在 RAM 中，读取速度比访问磁盘快得多，这是缓存好用的根本原因。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- Redis 是生产环境中存储 session 的常用首选方案，因为它读写速度快，并且原生支持 key 的过期（expiration）机制。（[90:23](https://youtu.be/oYxTTirKY8M?t=5423)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[in-memory-vs-distributed-cache]]
- [[ram-cost-scarcity]]
- [[session-storage-options]]
%% ytkb:end %%
