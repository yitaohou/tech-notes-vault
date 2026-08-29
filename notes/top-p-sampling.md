---
title: Top-P (Nucleus) Sampling
aliases: []
tags:
- concept
summary: 选择累积概率超过阈值 P 的最小 token 集合进行采样的技术，例如 P=0.9 表示只考虑累计占90%概率质量的 token。
created: '2026-08-26'
updated: '2026-08-26'
---

# Top-P (Nucleus) Sampling

%% ytkb:def %%
选择累积概率超过阈值 P 的最小 token 集合进行采样的技术，例如 P=0.9 表示只考虑累计占90%概率质量的 token。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- top-P sampling 选取累积概率超过阈值 P 的最小 token 集合进行采样，例如 P 取 0.9 意味着只考虑合计占90%概率质量的 token。（[06:00](https://youtu.be/JV3pL1_mn2M?t=360)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[temperature-sampling]]
- [[top-k-sampling]]
%% ytkb:end %%
