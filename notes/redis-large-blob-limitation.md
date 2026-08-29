---
title: Redis Large Blob Limitation
aliases: []
tags:
- concept
summary: Redis 并非为流式传输大体积二进制数据（如视频、图片文件字节）而设计，在 Redis 中缓存大文件字节通常是错误做法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Redis Large Blob Limitation

%% ytkb:def %%
Redis 并非为流式传输大体积二进制数据（如视频、图片文件字节）而设计，在 Redis 中缓存大文件字节通常是错误做法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 把几十上百 MB 的视频或图片字节直接存进 Redis 通常是错误的做法，因为这类内存很昂贵，而且 Redis 本身并不是为流式传输大体积 blob 设计的。（[39:09](https://youtu.be/Qa-7iWxDz1A?t=2349)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cdn-edge-asset-caching]]
- [[redis-in-ram-key-value-cache]]
%% ytkb:end %%
