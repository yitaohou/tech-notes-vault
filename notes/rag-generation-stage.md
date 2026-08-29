---
title: RAG Generation Stage
aliases: []
tags:
- concept
summary: 生成阶段是RAG流程的最后一步，把重排筛选出的最相关片段与用户问题一起发送给大模型，由大模型据此生成最终答案。
created: '2026-08-26'
updated: '2026-08-26'
---

# RAG Generation Stage

%% ytkb:def %%
生成阶段是RAG流程的最后一步，把重排筛选出的最相关片段与用户问题一起发送给大模型，由大模型据此生成最终答案。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 生成阶段会把重排后筛选出的3个最相关片段连同用户问题一起提交给大模型，由大模型产出最终答案，至此整个RAG流程结束。（[15:04](https://youtu.be/WWdlme1EAGI?t=904)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cross-encoder-rerank]]
- [[rag-pipeline-two-phases]]
%% ytkb:end %%
