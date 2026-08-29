---
title: RAG Indexing
aliases: []
tags:
- concept
summary: 索引是 RAG 数据准备阶段的第二个环节，通过 embedding 把片段文本转换为向量，再将文本与向量一起存入向量数据库。
created: '2026-08-26'
updated: '2026-08-26'
---

# RAG Indexing

%% ytkb:def %%
索引是 RAG 数据准备阶段的第二个环节，通过 embedding 把片段文本转换为向量，再将文本与向量一起存入向量数据库。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 索引环节包含两步：先用 embedding 把每个片段文本转换为对应向量，再将片段文本及其向量一起存储进向量数据库。（[03:00](https://youtu.be/WWdlme1EAGI?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[document-chunking]]
- [[embedding]]
- [[vector-database]]
%% ytkb:end %%
