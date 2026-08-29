---
title: Sparse Model Parameter Count Caveat
aliases: []
tags:
- concept
summary: 对于含大量零值参数的稀疏模型而言，参数总数可能误导对实际计算量的判断。
created: '2026-08-26'
updated: '2026-08-26'
---

# Sparse Model Parameter Count Caveat

%% ytkb:def %%
对于含大量零值参数的稀疏模型而言，参数总数可能误导对实际计算量的判断。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-llm-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 参数数量对稀疏模型（含大量零值参数）可能有误导性，一个大型稀疏模型所需的计算量可能反而少于一个较小的密集模型。（[03:00](https://youtu.be/JV3pL1_mn2M?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[model-parameter-capacity]]
%% ytkb:end %%
