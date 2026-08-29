---
title: Catastrophic Forgetting
aliases: []
tags:
- concept
summary: 模型在 sequential fine-tuning 中因先后学习不同任务而丧失早期任务能力的现象。
created: '2026-08-26'
updated: '2026-08-26'
---

# Catastrophic Forgetting

%% ytkb:def %%
模型在 sequential fine-tuning 中因先后学习不同任务而丧失早期任务能力的现象。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- sequential fine-tuning（先训练任务 A、再训练任务 B）可能导致 catastrophic forgetting，即模型在学习任务 B 后丧失在任务 A 上的能力。（[48:04](https://youtu.be/JV3pL1_mn2M?t=2884)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[multi-task-fine-tuning-options]]
%% ytkb:end %%
