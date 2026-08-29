---
title: Retrieval Augmented Generation (RAG)
aliases: []
tags:
- concept
summary: RAG（检索增强生成）是一种先从资料库中检索相关内容、再基于检索到的内容生成答案的 AI 问答技术方案。
created: '2026-08-26'
updated: '2026-08-26'
---

# Retrieval Augmented Generation (RAG)

%% ytkb:def %%
RAG（检索增强生成）是一种先从资料库中检索相关内容、再基于检索到的内容生成答案的 AI 问答技术方案。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- RAG 全称 Retrieval Augmented Generation，核心流程分两步：先从资料库中检索相关内容，再基于这些内容生成答案，因此得名检索增强生成。（[00:00](https://youtu.be/WWdlme1EAGI?t=0)）
- RAG 是目前最常用的 AI 问答方案之一，许多企业内部知识助手和智能客服系统都基于该技术构建。（[00:00](https://youtu.be/WWdlme1EAGI?t=0)）
- RAG 的核心机制是根据用户问题在大量文档片段中检索出真正相关的少数片段（如百页手册中的三个片段），只把这些片段和问题一起发给大模型，而不是把整份文档发给它。（[03:00](https://youtu.be/WWdlme1EAGI?t=180)）
%% ytkb:end %%

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 可以把 RAG 理解为一种针对每次查询构建特定上下文的技术，用来把模型和它训练时没见过、或者已经遗忘的信息连接起来。（[30:02](https://youtu.be/JV3pL1_mn2M?t=1802)）
%% ytkb:end %%

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- RAG 本质是通过语义检索获取大模型本身不掌握的 private data（如公司退货政策），把这些专有信息喂给 AI agent 使用。（[12:39](https://youtu.be/CyLYY_xb5bQ?t=759)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[document-chunking]]
- [[full-document-context-injection]]
- [[rag-retrieval]]
- [[rag-retriever]]
- [[rag-two-phase-pipeline]]
- [[vector-database-rag]]
%% ytkb:end %%
