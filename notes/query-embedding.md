---
title: Query Embedding
aliases: []
tags:
- concept
summary: 召回环节中，将用户提出的问题通过 embedding 模型转换为向量的步骤，用于后续在向量数据库中检索。
created: '2026-08-26'
updated: '2026-08-26'
---

# Query Embedding

%% ytkb:def %%
召回环节中，将用户提出的问题通过 embedding 模型转换为向量的步骤，用于后续在向量数据库中检索。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 召回流程中，用户的问题会先被发送给 embedding 模型转换为向量，再用该向量去向量数据库中查询相关片段。（[09:03](https://youtu.be/WWdlme1EAGI?t=543)）
%% ytkb:end %%

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 查询向量必须使用与文档 embedding 相同的模型来生成，才能保证两者处于同一语义空间，从而准确检索最相近的 chunk。（[33:02](https://youtu.be/JV3pL1_mn2M?t=1982)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[embedding-based-retrieval]]
- [[embedding-model]]
- [[rag-retrieval]]
%% ytkb:end %%
