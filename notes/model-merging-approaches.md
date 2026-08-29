---
title: Model Merging Approaches
aliases: []
tags:
- concept
summary: 将多个已微调模型合并为一个模型的几种具体方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Model Merging Approaches

%% ytkb:def %%
将多个已微调模型合并为一个模型的几种具体方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-model-selection-deployment]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 常见的 model merging 方法包括：summing（直接把各模型权重值相加，最常用）、layer stacking（也叫 Franken merging，从不同模型中取不同层堆叠起来）、以及 concatenation（直接拼接参数，因不能降低内存占用而不太推荐）。（[48:04](https://youtu.be/JV3pL1_mn2M?t=2884)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[model-merging]]
%% ytkb:end %%
