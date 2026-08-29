---
title: Inference Uses Only Forward Pass
aliases: []
tags:
- concept
summary: 推理阶段只执行神经网络的前向传播，不涉及权重更新。
created: '2026-08-26'
updated: '2026-08-26'
---

# Inference Uses Only Forward Pass

%% ytkb:def %%
推理阶段只执行神经网络的前向传播，不涉及权重更新。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- inference 阶段只执行 forward pass，而 training 阶段需要同时执行 forward pass 和 backward pass。（[45:04](https://youtu.be/JV3pL1_mn2M?t=2704)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[backpropagation]]
%% ytkb:end %%
