---
title: LoRA (Low-Rank Adaptation)
aliases: []
tags:
- concept
summary: LoRA 是最流行的 adapter-based PEFT 方法，通过低秩矩阵分解实现高效微调。
created: '2026-08-26'
updated: '2026-09-02'
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

%% ytkb:video:HdkhI6VyQD0 %%
### 来自 [[2026-09-01-臨床小型語言模型的運作原理]]
- 研究团队透过 LoRA 技术对 Med42-8B 进行高效率参数微调，使小模型不需借助超级计算机也能完成训练。（[03:00](https://youtu.be/HdkhI6VyQD0?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[full-fine-tuning]]
- [[knowledge-distillation]]
- [[peft]]
- [[peft-method-categories]]
%% ytkb:end %%
