---
title: Knowledge Distillation
aliases: []
tags:
- concept
summary: Distillation 是一种模型压缩技术，通过训练一个更小的模型去模仿一个更大模型的行为。
created: '2026-08-26'
updated: '2026-09-02'
---

# Knowledge Distillation

%% ytkb:def %%
Distillation 是一种模型压缩技术，通过训练一个更小的模型去模仿一个更大模型的行为。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- Distillation 通过训练一个更小的模型来模仿一个更大模型的行为，从而实现模型压缩。（[63:05](https://youtu.be/JV3pL1_mn2M?t=3785)）
%% ytkb:end %%

%% ytkb:video:HdkhI6VyQD0 %%
### 来自 [[2026-09-01-臨床小型語言模型的運作原理]]
- 该临床研究中的模型蒸馏，是让算力强大的 Gemini 2.0 Flash 担任教师模型生成教学用伪标签，再将其推论能力转移给一个80亿参数的小模型 Med42-8B。（[03:00](https://youtu.be/HdkhI6VyQD0?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[lora]]
- [[med42-8b-model]]
- [[model-compression]]
%% ytkb:end %%
