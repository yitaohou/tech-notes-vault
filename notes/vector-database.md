---
title: Vector Database
aliases: []
tags:
- concept
summary: 向量数据库是专门用于存储和查询向量的数据库，针对向量存储做了优化，并提供向量相似度计算等相关函数。
created: '2026-08-26'
updated: '2026-08-26'
---

# Vector Database

%% ytkb:def %%
向量数据库是专门用于存储和查询向量的数据库，针对向量存储做了优化，并提供向量相似度计算等相关函数。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 向量数据库针对向量存储做了专门优化，并提供计算向量相似度等函数，方便检索和使用向量。（[06:00](https://youtu.be/WWdlme1EAGI?t=360)）
- 向量数据库中不仅要存储向量本身，还必须存储对应的原始文本，因为最终需要提取给大模型的是原始文本而非向量，所以其表格通常至少包含原始文本和向量两列。（[06:00](https://youtu.be/WWdlme1EAGI?t=360)）
- 向量数据库中存储的内容包括每个片段的原始文本以及它对应的向量。（[03:00](https://youtu.be/WWdlme1EAGI?t=180)）
%% ytkb:end %%

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 向量数据库通常使用各种启发式方法把向量组织成桶（buckets）、树（trees）或图（graphs），以提高相似向量被存储在彼此邻近位置的概率。（[33:02](https://youtu.be/JV3pL1_mn2M?t=1982)）
%% ytkb:end %%

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 传统关系型数据表用行列结构存储数据（类似 Excel 表格，每列代表一个 feature，每行代表一条 entry），但像退款政策这类非结构化文本内容（段落或 PDF）不适合这种表格格式，因此需要存入向量数据库。（[03:00](https://youtu.be/CyLYY_xb5bQ?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[approximate-nearest-neighbor-search]]
- [[embedding]]
- [[rag-indexing]]
- [[rag-retrieval-process]]
%% ytkb:end %%
