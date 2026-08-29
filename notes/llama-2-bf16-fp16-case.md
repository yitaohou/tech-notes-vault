---
title: Llama 2 bf16 vs fp16 Case
aliases: []
tags:
- concept
summary: Llama 2 发布时权重针对 bf16 格式优化，若改用 fp16 加载会导致质量明显下降的真实案例。
created: '2026-08-26'
updated: '2026-08-26'
---

# Llama 2 bf16 vs fp16 Case

%% ytkb:def %%
Llama 2 发布时权重针对 bf16 格式优化，若改用 fp16 加载会导致质量明显下降的真实案例。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- Llama 2 发布时其权重针对 bf16 格式做了优化，如果改用 fp16 格式加载模型，会导致输出质量显著变差。（[45:04](https://youtu.be/JV3pL1_mn2M?t=2704)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[precision-reduction-risk]]
%% ytkb:end %%
