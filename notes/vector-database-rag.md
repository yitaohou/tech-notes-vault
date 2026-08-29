---
title: Vector Database (RAG)
aliases: []
tags:
- concept
summary: 向量数据库用于存储片段向量，并根据查询向量检索出最相似的片段。
created: '2026-08-26'
updated: '2026-08-26'
---

# Vector Database (RAG)

%% ytkb:def %%
向量数据库用于存储片段向量，并根据查询向量检索出最相似的片段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 生成的片段向量会被存入向量数据库，至此提问前的知识库构建准备工作完成，等待用户使用。（[15:04](https://youtu.be/WWdlme1EAGI?t=904)）
%% ytkb:end %%

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- FAQ、政策文档这类非结构化的段落型数据不易在表格中检索，更适合存入向量数据库并通过语义相似度检索获取相关信息。（[12:20](https://youtu.be/CyLYY_xb5bQ?t=740)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[embedding-based-retrieval]]
- [[embedding-model]]
- [[rag-recall]]
- [[retrieval-augmented-generation]]
%% ytkb:end %%
