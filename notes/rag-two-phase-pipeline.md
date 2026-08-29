---
title: RAG Two-Phase Pipeline
aliases: []
tags:
- concept
summary: RAG 整体流程分为数据准备和回答两大部分，前者在用户提问前完成，后者在用户提问后触发。
created: '2026-08-26'
updated: '2026-08-26'
---

# RAG Two-Phase Pipeline

%% ytkb:def %%
RAG 整体流程分为数据准备和回答两大部分，前者在用户提问前完成，后者在用户提问后触发。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- RAG 整体流程包含两部分：用户提问前的数据准备部分（含分片和索引两个环节），以及用户提问后的回答部分（含召回、重排和生成三个环节）。（[03:00](https://youtu.be/WWdlme1EAGI?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[document-chunking]]
- [[rag-generation]]
- [[rag-indexing]]
- [[rag-reranking]]
- [[rag-retrieval]]
%% ytkb:end %%
