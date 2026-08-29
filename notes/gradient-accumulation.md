---
title: Gradient Accumulation
aliases: []
tags:
- concept
summary: 在显存受限时，通过累积多个小 batch 的梯度后再统一更新参数，从而模拟大 batch 训练效果的技术。
created: '2026-08-26'
updated: '2026-08-26'
---

# Gradient Accumulation

%% ytkb:def %%
在显存受限时，通过累积多个小 batch 的梯度后再统一更新参数，从而模拟大 batch 训练效果的技术。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 梯度累积（gradient accumulation）可用于缓解小 batch size 训练时的不稳定问题。（[51:04](https://youtu.be/JV3pL1_mn2M?t=3064)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[batch-size-fine-tuning-hyperparameter]]
%% ytkb:end %%
