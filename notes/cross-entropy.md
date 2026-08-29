---
title: Cross Entropy
aliases: []
tags:
- concept
summary: Cross entropy 是训练自回归语言模型时常用的指标，衡量模型预测序列中下一个 token 的准确程度。
created: '2026-08-26'
updated: '2026-08-26'
---

# Cross Entropy

%% ytkb:def %%
Cross entropy 是训练自回归语言模型时常用的指标，衡量模型预测序列中下一个 token 的准确程度。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-llm-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 大多数自回归语言模型的训练使用 cross entropy（或与其相关的 perplexity）作为指标，本质是衡量模型预测下一个 token 的能力。（[09:01](https://youtu.be/JV3pL1_mn2M?t=541)）
- 语言模型的训练目标是学习训练数据的概率分布，模型对该分布学得越好，预测下一个 token 的能力就越强，对应的 cross entropy 就越低。（[09:01](https://youtu.be/JV3pL1_mn2M?t=541)）
- 一个完美训练的模型，其 cross entropy 会等于训练数据本身的 entropy，此时模型分布与真实数据分布之间的 KL divergence 为零。（[09:01](https://youtu.be/JV3pL1_mn2M?t=541)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[entropy-information-theory]]
- [[perplexity]]
%% ytkb:end %%
