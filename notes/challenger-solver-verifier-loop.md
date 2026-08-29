---
title: Challenger-Solver-Verifier Loop
aliases: []
tags:
- concept
summary: 一种数据生成机制，挑战者根据求解器和验证器的反馈迭代更新提示词，产出强求解器能完成而弱求解器会失败的题目。
created: '2026-08-26'
updated: '2026-08-26'
---

# Challenger-Solver-Verifier Loop

%% ytkb:def %%
一种数据生成机制，挑战者根据求解器和验证器的反馈迭代更新提示词，产出强求解器能完成而弱求解器会失败的题目。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-training-data]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- 该方法生成的合成数据只用来微调弱模型、不会迭代改进强模型，因此更接近间接的知识蒸馏，自我改进的属性并不强。（[12:08](https://youtu.be/z_F0z7wF5XU?t=728)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[knowledge-distillation]]
%% ytkb:end %%
