---
title: Multi-Task Fine-Tuning Options
aliases: []
tags:
- concept
summary: 为一个模型微调以支持多个任务时可选的几种策略。
created: '2026-08-26'
updated: '2026-08-26'
---

# Multi-Task Fine-Tuning Options

%% ytkb:def %%
为一个模型微调以支持多个任务时可选的几种策略。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 针对多任务微调，可选择 simultaneous fine-tuning（把所有任务的数据一起训练，难度更高、需要更多数据）、sequential fine-tuning（先训练任务 A 再训练任务 B）或 model merging（分别微调后再合并模型）。（[48:04](https://youtu.be/JV3pL1_mn2M?t=2884)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[catastrophic-forgetting]]
- [[model-merging]]
%% ytkb:end %%
