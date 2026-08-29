---
title: Quantization Memory Example (13B Model)
aliases: []
tags:
- concept
summary: 一个具体计算示例：130 亿参数模型在不同位宽下所需内存的对比。
created: '2026-08-26'
updated: '2026-08-26'
---

# Quantization Memory Example (13B Model)

%% ytkb:def %%
一个具体计算示例：130 亿参数模型在不同位宽下所需内存的对比。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 以 130 亿参数模型为例，使用 32-bit 浮点数时每个参数占 4 字节，总内存约 52GB；若降至 16-bit，内存需求降至约 26GB。（[45:04](https://youtu.be/JV3pL1_mn2M?t=2704)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[quantization]]
%% ytkb:end %%
