---
title: Sequential Processing Bottleneck
aliases: []
tags:
- concept
summary: 早期 encoder-decoder 架构在输入处理和输出生成阶段都按 token 顺序依次进行，导致长序列处理速度缓慢的问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# Sequential Processing Bottleneck

%% ytkb:def %%
早期 encoder-decoder 架构在输入处理和输出生成阶段都按 token 顺序依次进行，导致长序列处理速度缓慢的问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-llm-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- encoder-decoder 架构的输入处理和输出生成都是按 token 顺序串行完成的，因此处理长序列时速度很慢。（[03:00](https://youtu.be/JV3pL1_mn2M?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[encoder-decoder-architecture]]
- [[transformer-parallel-processing]]
%% ytkb:end %%
