---
title: Training vs Inference Hardware Requirements
aliases: []
tags:
- concept
summary: 训练与推理阶段对硬件资源的需求存在显著差异。
created: '2026-08-26'
updated: '2026-08-26'
---

# Training vs Inference Hardware Requirements

%% ytkb:def %%
训练与推理阶段对硬件资源的需求存在显著差异。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-engineering-fundamentals]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 训练由于需要执行反向传播（back prop），通常比推理更消耗内存、执行难度更高，且倾向使用更低精度（更高数值精度需求）；推理则因用户在等待响应，往往更看重 latency 而非 throughput。（[63:05](https://youtu.be/JV3pL1_mn2M?t=3785)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-accelerator]]
%% ytkb:end %%
