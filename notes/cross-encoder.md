---
title: Cross Encoder
aliases: []
tags:
- concept
summary: Cross encoder 是重排阶段常用的一种模型，用于精确计算每个候选片段与用户问题之间的相似度。
created: '2026-08-26'
updated: '2026-08-26'
---

# Cross Encoder

%% ytkb:def %%
Cross encoder 是重排阶段常用的一种模型，用于精确计算每个候选片段与用户问题之间的相似度。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 相较于向量相似度方法，cross encoder 的计算成本更高、耗时更长，但准确率也高得多，因此适合在重排阶段做精挑细选。（[12:03](https://youtu.be/WWdlme1EAGI?t=723)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rag-rerank]]
- [[vector-similarity]]
%% ytkb:end %%
