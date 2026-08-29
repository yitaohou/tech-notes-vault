---
title: Autoregressive Generation Bottleneck
aliases: []
tags:
- concept
summary: 指语言模型自回归（autoregressive）逐个 token 顺序生成文本的特性所造成的推理顺序性瓶颈。
created: '2026-08-26'
updated: '2026-08-26'
---

# Autoregressive Generation Bottleneck

%% ytkb:def %%
指语言模型自回归（autoregressive）逐个 token 顺序生成文本的特性所造成的推理顺序性瓶颈。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 语言模型的自回归特性使其必须逐个 token 顺序生成文本，这构成了推理速度的顺序性瓶颈，多种技术专门用于缓解这一限制。（[63:05](https://youtu.be/JV3pL1_mn2M?t=3785)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[parallel-decoding]]
- [[prompt-lookup-decoding]]
- [[speculative-decoding]]
%% ytkb:end %%
