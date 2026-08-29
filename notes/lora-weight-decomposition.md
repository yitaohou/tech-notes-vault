---
title: LoRA Weight Matrix Decomposition
aliases: []
tags:
- concept
summary: LoRA 通过将权重矩阵分解为更小矩阵的乘积来实现参数高效微调。
created: '2026-08-26'
updated: '2026-08-26'
---

# LoRA Weight Matrix Decomposition

%% ytkb:def %%
LoRA 通过将权重矩阵分解为更小矩阵的乘积来实现参数高效微调。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 对于维度为 n×m 的权重矩阵，LoRA 先选定一个更小的秩 R，再构造 n×R 的矩阵 A 和 R×m 的矩阵 B；微调时只更新 A 和 B，原始权重保持冻结。（[48:04](https://youtu.be/JV3pL1_mn2M?t=2884)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[lora]]
%% ytkb:end %%
