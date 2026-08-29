---
title: LoRA (Low-Rank Adaptation)
aliases: []
tags:
- concept
summary: LoRA 是最流行的 adapter-based PEFT 方法，通过低秩矩阵分解实现高效微调。
created: '2026-08-26'
updated: '2026-08-26'
---

# LoRA (Low-Rank Adaptation)

%% ytkb:def %%
LoRA 是最流行的 adapter-based PEFT 方法，通过低秩矩阵分解实现高效微调。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 与传统 adapter 不同，LoRA 引入额外参数但不会增加推理延迟，因为它的模块可以合并回原始层，而不是新增层。（[48:04](https://youtu.be/JV3pL1_mn2M?t=2884)）
- LoRA 是文中提到的一种典型 PEFT 方法，常用于数据量有限时的微调场景。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[full-fine-tuning]]
- [[peft]]
- [[peft-method-categories]]
%% ytkb:end %%
