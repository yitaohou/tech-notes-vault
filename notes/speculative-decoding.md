---
title: Speculative Decoding
aliases: []
tags:
- concept
summary: Speculative decoding 使用一个更快但能力较弱的模型生成候选 token，再由目标模型进行验证的推理加速技术。
created: '2026-08-26'
updated: '2026-08-26'
---

# Speculative Decoding

%% ytkb:def %%
Speculative decoding 使用一个更快但能力较弱的模型生成候选 token，再由目标模型进行验证的推理加速技术。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- Speculative decoding 就像让一个助理起草回复、再由主管快速审核批准一样：用更快的小模型生成候选 token，再交由目标大模型验证。（[63:05](https://youtu.be/JV3pL1_mn2M?t=3785)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[autoregressive-generation-bottleneck]]
- [[parallel-decoding]]
%% ytkb:end %%
