---
title: LoRA Rank and Module Selection Tradeoff
aliases: []
tags:
- concept
summary: LoRA 的效率同时取决于所选的秩大小以及应用于哪些权重矩阵。
created: '2026-08-26'
updated: '2026-08-26'
---

# LoRA Rank and Module Selection Tradeoff

%% ytkb:def %%
LoRA 的效率同时取决于所选的秩大小以及应用于哪些权重矩阵。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- LoRA 主要应用于 Transformer 的 attention 模块，其效率高低取决于所选的 rank 大小以及具体应用在哪些矩阵上。（[48:04](https://youtu.be/JV3pL1_mn2M?t=2884)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[lora]]
- [[lora-weight-decomposition]]
%% ytkb:end %%
