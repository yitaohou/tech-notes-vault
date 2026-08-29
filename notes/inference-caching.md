---
title: Inference Caching
aliases: []
tags:
- concept
summary: 推理阶段的缓存优化技术统称，包括KV caching和prompt caching等，用于降低性能和成本开销。
created: '2026-08-26'
updated: '2026-08-26'
---

# Inference Caching

%% ytkb:def %%
推理阶段的缓存优化技术统称，包括KV caching和prompt caching等，用于降低性能和成本开销。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- inference caching对多步骤流程（如Chain of Thought推理，或需要检索、网络搜索等耗时操作的查询）尤其有价值。（[69:07](https://youtu.be/JV3pL1_mn2M?t=4147)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cache-eviction-policy]]
- [[kv-caching]]
- [[prompt-caching]]
%% ytkb:end %%
