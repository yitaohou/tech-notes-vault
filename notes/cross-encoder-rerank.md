---
title: Cross-Encoder Rerank
aliases: []
tags:
- concept
summary: 重排是RAG回答阶段的第二步，使用cross-encoder模型对召回的候选片段重新打分排序，筛选出相关程度最高的少数片段。
created: '2026-08-26'
updated: '2026-08-26'
---

# Cross-Encoder Rerank

%% ytkb:def %%
重排是RAG回答阶段的第二步，使用cross-encoder模型对召回的候选片段重新打分排序，筛选出相关程度最高的少数片段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 重排阶段把召回得到的10个候选片段送入cross-encoder模型，从中筛选出3个与用户问题相关程度最高的片段。（[15:04](https://youtu.be/WWdlme1EAGI?t=904)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rag-generation-stage]]
- [[rag-recall]]
%% ytkb:end %%
