---
title: Cache-Aside Pattern
aliases: []
tags:
- concept
summary: 一种读缓存模式：请求先查 cache，命中则直接返回；未命中则查数据库，再把结果写入 cache 供后续请求使用。
created: '2026-08-26'
updated: '2026-08-26'
---

# Cache-Aside Pattern

%% ytkb:def %%
一种读缓存模式：请求先查 cache，命中则直接返回；未命中则查数据库，再把结果写入 cache 供后续请求使用。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- cache-aside 模式的核心逻辑是先判断 key（如 file123）是否存在于 cache 中，存在则直接返回，避免访问数据库；不存在则查数据库、写入 cache 后再返回给用户，使下一次同样的请求命中缓存变快。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
- cache-aside 是后端实现缓存机制时非常常见的通用模式，值得熟练掌握。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cdn-origin-bypass]]
- [[file-metadata-object-storage-split]]
%% ytkb:end %%
