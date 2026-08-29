---
title: RAG Retrieval Process
aliases: []
tags:
- concept
summary: RAG检索流程指先将用户问题做embedding得到向量，再通过向量相似度找出相关文本片段，最后将这些相关文本与原始问题一起提交给大模型生成回答。
created: '2026-08-26'
updated: '2026-08-26'
---

# RAG Retrieval Process

%% ytkb:def %%
RAG检索流程指先将用户问题做embedding得到向量，再通过向量相似度找出相关文本片段，最后将这些相关文本与原始问题一起提交给大模型生成回答。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- RAG回答用户问题时，先把用户问题embedding成向量，再依据向量相似度检索出相关的原始文本，最后将这些相关文本与用户问题一并提交给大模型生成答案。（[06:00](https://youtu.be/WWdlme1EAGI?t=360)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[embedding]]
- [[vector-database]]
%% ytkb:end %%
