---
title: Precision Reduction Risk
aliases: []
tags:
- concept
summary: 降低数值精度可能导致模型数值发生变化或产生误差，因此应按模型训练时的目标格式加载。
created: '2026-08-26'
updated: '2026-08-26'
---

# Precision Reduction Risk

%% ytkb:def %%
降低数值精度可能导致模型数值发生变化或产生误差，因此应按模型训练时的目标格式加载。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 降低数值精度可能导致数值发生变化或产生误差，所以加载模型时应使用其训练时所用的目标格式，而非随意转换。（[45:04](https://youtu.be/JV3pL1_mn2M?t=2704)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[llama-2-bf16-fp16-case]]
- [[numerical-format-range-precision]]
%% ytkb:end %%
