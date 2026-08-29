---
title: Transformer Prefill and Decode Steps
aliases: []
tags:
- concept
summary: Transformer 推理分两步：pre-fill 阶段并行处理所有输入 token 生成中间状态，decode 阶段逐个生成输出 token。
created: '2026-08-26'
updated: '2026-08-26'
---

# Transformer Prefill and Decode Steps

%% ytkb:def %%
Transformer 推理分两步：pre-fill 阶段并行处理所有输入 token 生成中间状态，decode 阶段逐个生成输出 token。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- Transformer 推理分两步进行：pre-fill 阶段并行处理全部输入 token 生成中间状态，decode 阶段则一次生成一个输出 token。（[03:00](https://youtu.be/JV3pL1_mn2M?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[attention-mechanism]]
- [[transformer-parallel-processing]]
%% ytkb:end %%
