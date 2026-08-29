---
title: Embedding Model
aliases: []
tags:
- concept
summary: embedding模型是专门用于将文本转换为向量的模型，区别于GPT-4o、DeepSeek等通用生成式对话模型。
created: '2026-08-26'
updated: '2026-08-26'
---

# Embedding Model

%% ytkb:def %%
embedding模型是专门用于将文本转换为向量的模型，区别于GPT-4o、DeepSeek等通用生成式对话模型。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 完成embedding操作的是专门的embedding模型，而不是GPT-4o、DeepSeek这类通用对话大模型。（[06:00](https://youtu.be/WWdlme1EAGI?t=360)）
- 索引环节中，所有分片会被送入embedding模型，由其为每个片段产出对应的向量。（[15:04](https://youtu.be/WWdlme1EAGI?t=904)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[embedding]]
- [[text-chunking-rag]]
- [[vector-database-rag]]
%% ytkb:end %%
