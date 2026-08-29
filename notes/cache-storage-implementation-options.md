---
title: Cache Storage Implementation Options
aliases: []
tags:
- concept
summary: 实现inference caching时可选的存储方案，速度与容量存在权衡。
created: '2026-08-26'
updated: '2026-08-26'
---

# Cache Storage Implementation Options

%% ytkb:def %%
实现inference caching时可选的存储方案，速度与容量存在权衡。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 缓存实现方案范围从速度快但容量有限的in-memory storage，到Postgres SQL、Redis这类数据库，需按需求权衡速度与容量。（[69:07](https://youtu.be/JV3pL1_mn2M?t=4147)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[inference-caching]]
%% ytkb:end %%
