---
title: RAG Retrieval
aliases: []
tags:
- concept
summary: 召回（retrieval）是 RAG 回答阶段的第一个环节，指根据用户问题在向量数据库中检索相关片段。
created: '2026-08-26'
updated: '2026-08-26'
---

# RAG Retrieval

%% ytkb:def %%
召回（retrieval）是 RAG 回答阶段的第一个环节，指根据用户问题在向量数据库中检索相关片段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 召回是回答部分的第一个环节，发生在用户提问之后，其后依次是重排和生成两个环节。（[03:00](https://youtu.be/WWdlme1EAGI?t=180)）
- 召回（retrieval）是指在用户提出问题后，搜索与该问题相关片段内容的过程，是索引阶段完成之后才发生的环节。（[09:03](https://youtu.be/WWdlme1EAGI?t=543)）
%% ytkb:end %%

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- querying 是发送搜索查询、检索出与该查询相关数据的过程。（[30:02](https://youtu.be/JV3pL1_mn2M?t=1802)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[query-embedding]]
- [[rag-generation]]
- [[rag-indexing-pipeline]]
- [[rag-reranking]]
- [[rag-two-phase-pipeline]]
- [[retriever-two-functions]]
- [[top-k-retrieval]]
%% ytkb:end %%
