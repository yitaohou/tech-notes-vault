---
title: Mixed Precision Training
aliases: []
tags:
- concept
summary: 混合精度训练指训练过程中部分操作使用较高精度（如 32-bit）、部分操作使用较低精度（如 16-bit 或 8-bit）的方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Mixed Precision Training

%% ytkb:def %%
混合精度训练指训练过程中部分操作使用较高精度（如 32-bit）、部分操作使用较低精度（如 16-bit 或 8-bit）的方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- training 对数值精度更敏感，因此通常采用 mixed precision：部分运算使用 32-bit 等高精度，另一部分使用 16-bit 或 8-bit 等低精度。（[45:04](https://youtu.be/JV3pL1_mn2M?t=2704)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[inference-low-bit-precision]]
%% ytkb:end %%
