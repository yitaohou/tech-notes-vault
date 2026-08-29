---
title: LoRA Inference-Time Merging
aliases: []
tags:
- concept
summary: 推理阶段将 LoRA 训练得到的低秩矩阵合并回原始权重的方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# LoRA Inference-Time Merging

%% ytkb:def %%
推理阶段将 LoRA 训练得到的低秩矩阵合并回原始权重的方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 推理时，LoRA 的矩阵 A 和 B 相乘后加回原始权重，因此不会引入额外的推理计算开销。（[48:04](https://youtu.be/JV3pL1_mn2M?t=2884)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[lora]]
- [[lora-weight-decomposition]]
%% ytkb:end %%
