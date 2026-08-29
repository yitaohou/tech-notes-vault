---
title: Document Chunking
aliases: []
tags:
- concept
summary: 文档切分（chunking）是 RAG 流程中的预处理步骤，指将长文档拆分为多个较小片段，便于后续检索出与问题相关的部分。
created: '2026-08-26'
updated: '2026-08-26'
---

# Document Chunking

%% ytkb:def %%
文档切分（chunking）是 RAG 流程中的预处理步骤，指将长文档拆分为多个较小片段，便于后续检索出与问题相关的部分。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- RAG 解决长文档无法直接输入模型问题的第一步，是把整个文档切分为多个片段（chunks）。（[00:00](https://youtu.be/WWdlme1EAGI?t=0)）
- 分片就是把一份文档切分成多个片段，是数据准备阶段的第一步，完成后进入索引环节。（[03:00](https://youtu.be/WWdlme1EAGI?t=180)）
- 文档分片的常见方式包括按字数（例如每 1000 字一个片段）、按段落、按章节、按页码等多种切分方法。（[03:00](https://youtu.be/WWdlme1EAGI?t=180)）
%% ytkb:end %%

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 如果直接检索整份文档（文档长度可能从 10 个 token 到上百万 token 不等），上下文会变得任意长，可能超出模型的上下文窗口，因此通常需要把文档切分成更小的 chunk。（[30:02](https://youtu.be/JV3pL1_mn2M?t=1802)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[context-window-limits-large-models]]
- [[full-document-context-injection]]
- [[rag-indexing]]
- [[rag-two-phase-pipeline]]
- [[retrieval-augmented-generation]]
%% ytkb:end %%
