---
title: RAG 召回（Recall）阶段
aliases: []
tags:
- concept
summary: 召回是 RAG 流程中的初筛阶段，使用向量相似度等低成本方法从全部文本片段中挑出与用户问题最相似的一批候选片段。
created: '2026-08-26'
updated: '2026-08-26'
---

# RAG 召回（Recall）阶段

%% ytkb:def %%
召回是 RAG 流程中的初筛阶段，使用向量相似度等低成本方法从全部文本片段中挑出与用户问题最相似的一批候选片段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 召回阶段会从所有文本片段中挑选出与用户问题最相似的10个片段，作为下一步重排阶段的输入。（[12:03](https://youtu.be/WWdlme1EAGI?t=723)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rag-rerank]]
- [[vector-similarity]]
%% ytkb:end %%
