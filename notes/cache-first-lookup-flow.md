---
title: Cache-First Lookup Flow
aliases: []
tags:
- concept
summary: 请求处理时优先查询缓存，命中则直接从缓存返回结果，避免访问关系型数据库和对象存储，从而降低延迟。
created: '2026-08-26'
updated: '2026-08-26'
---

# Cache-First Lookup Flow

%% ytkb:def %%
请求处理时优先查询缓存，命中则直接从缓存返回结果，避免访问关系型数据库和对象存储，从而降低延迟。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 请求先经过 gateway 转发给 file service，file service 优先查询缓存；如果对应文件已经在缓存中处于 warm 且可用状态，就直接从缓存返回文件，无需再访问关系型数据库或对象存储。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cdn-edge-asset-caching]]
- [[redis-in-ram-key-value-cache]]
%% ytkb:end %%
