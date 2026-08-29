---
title: Reinforcement Learning from Human Feedback (RLHF)
aliases: []
tags:
- concept
summary: 一种通过训练 reward model 为输出打分、再据此优化基础模型以最大化该分数的偏好对齐方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Reinforcement Learning from Human Feedback (RLHF)

%% ytkb:def %%
一种通过训练 reward model 为输出打分、再据此优化基础模型以最大化该分数的偏好对齐方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- RLHF 先训练一个根据人类偏好给输出打分的 reward model，再优化基础模型生成能最大化该分数的回应。（[06:00](https://youtu.be/JV3pL1_mn2M?t=360)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[best-of-n-sampling]]
- [[dpo]]
- [[preference-fine-tuning]]
%% ytkb:end %%
