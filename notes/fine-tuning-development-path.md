---
title: Practical Fine-Tuning Development Path
aliases: []
tags:
- concept
summary: 一套典型的实践性微调开发流程建议。
created: '2026-08-26'
updated: '2026-08-26'
---

# Practical Fine-Tuning Development Path

%% ytkb:def %%
一套典型的实践性微调开发流程建议。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 实践中典型的微调开发路径是：先用最便宜最快的模型测试微调代码是否能跑通，再用中等规模模型测试数据（若训练损失不随数据增多而下降说明有问题），然后用目标模型做实验摸清性能上限，最后绘制 price-performance frontier 并据此选择最合适的模型。（[48:04](https://youtu.be/JV3pL1_mn2M?t=2884)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[distillation-development-path]]
%% ytkb:end %%
