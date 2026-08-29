---
title: Prompt Loss Weight
aliases: []
tags:
- concept
summary: instruction fine-tuning 中控制 prompt 部分对训练损失贡献比例的超参数。
created: '2026-08-26'
updated: '2026-08-26'
---

# Prompt Loss Weight

%% ytkb:def %%
instruction fine-tuning 中控制 prompt 部分对训练损失贡献比例的超参数。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- prompt loss weight 决定 prompt 相对 response 对 loss 的贡献比例：设为 100% 时二者贡献相等，设为 0% 时模型只从 response 学习，默认值通常为 10%。（[51:04](https://youtu.be/JV3pL1_mn2M?t=3064)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[full-fine-tuning]]
%% ytkb:end %%
