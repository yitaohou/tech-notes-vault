---
title: Teacher Model Pseudo-Label Generation
aliases: []
tags:
- concept
summary: 蒸馏流程中由教师模型阅读大量真实病例、生成用于训练学生模型的伪标签的步骤。
created: '2026-09-02'
updated: '2026-09-02'
---

# Teacher Model Pseudo-Label Generation

%% ytkb:def %%
蒸馏流程中由教师模型阅读大量真实病例、生成用于训练学生模型的伪标签的步骤。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-training-data]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:HdkhI6VyQD0 %%
### 来自 [[2026-09-01-臨床小型語言模型的運作原理]]
- 教师模型 Gemini 2.0 Flash 阅读了2256份真实病例来生成教学用的伪标签，作为学生模型 Med42-8B 的训练数据来源。（[03:00](https://youtu.be/HdkhI6VyQD0?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[knowledge-distillation]]
- [[med42-8b-model]]
%% ytkb:end %%
