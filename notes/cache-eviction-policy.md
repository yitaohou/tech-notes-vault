---
title: Cache Eviction Policy
aliases: []
tags:
- concept
summary: 当缓存容量达到上限时，决定淘汰哪些缓存条目的规则，如LRU、LFU。
created: '2026-08-26'
updated: '2026-08-26'
---

# Cache Eviction Policy

%% ytkb:def %%
当缓存容量达到上限时，决定淘汰哪些缓存条目的规则，如LRU、LFU。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-caching-edge]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 随着规模扩大，需要设置eviction policy（如least recently used或least frequently used）来管理缓存大小。（[69:07](https://youtu.be/JV3pL1_mn2M?t=4147)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cache-storage-implementation-options]]
- [[inference-caching]]
%% ytkb:end %%
