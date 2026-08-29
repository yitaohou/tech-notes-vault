---
title: RAG Recall (Retrieval)
aliases: []
tags:
- concept
summary: 召回是RAG回答阶段的第一步，指根据用户问题向量从向量数据库中检索出若干候选相关片段。
created: '2026-08-26'
updated: '2026-08-26'
---

# RAG Recall (Retrieval)

%% ytkb:def %%
召回是RAG回答阶段的第一步，指根据用户问题向量从向量数据库中检索出若干候选相关片段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 召回阶段先由embedding模型把用户问题转换为向量，再交给向量数据库检索出10个与问题最相近的片段。（[15:04](https://youtu.be/WWdlme1EAGI?t=904)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cross-encoder-rerank]]
- [[embedding-model]]
- [[vector-database-rag]]
%% ytkb:end %%
