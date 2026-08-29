---
title: Encoder-Decoder Architecture
aliases: []
tags:
- concept
summary: 早期用于翻译等任务的神经网络架构，由处理输入的 encoder 和生成输出的 decoder 组成，两者都按 token 顺序依次处理。
created: '2026-08-26'
updated: '2026-08-26'
---

# Encoder-Decoder Architecture

%% ytkb:def %%
早期用于翻译等任务的神经网络架构，由处理输入的 encoder 和生成输出的 decoder 组成，两者都按 token 顺序依次处理。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-llm-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 传统 encoder-decoder 架构中，decoder 只能访问 encoder 对整个输入压缩后的表示，就像只靠一段书籍摘要去回答关于书本细节的问题。（[03:00](https://youtu.be/JV3pL1_mn2M?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[attention-mechanism]]
- [[sequential-processing-bottleneck]]
%% ytkb:end %%
