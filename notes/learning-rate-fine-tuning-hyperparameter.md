---
title: Learning Rate (Fine-Tuning)
aliases: []
tags:
- concept
summary: 微调中控制参数更新步长的核心超参数。
created: '2026-08-26'
updated: '2026-08-26'
---

# Learning Rate (Fine-Tuning)

%% ytkb:def %%
微调中控制参数更新步长的核心超参数。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 微调时若 loss curve 剧烈波动通常说明学习率过高；若 loss 稳定但下降极慢则说明学习率过低，一般做法是学习率从较大值开始随训练逐步降低。（[51:04](https://youtu.be/JV3pL1_mn2M?t=3064)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[batch-size-fine-tuning-hyperparameter]]
- [[epoch-count-fine-tuning]]
%% ytkb:end %%
