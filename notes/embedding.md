---
title: Embedding
aliases: []
tags:
- concept
summary: embedding是将文本转换为向量的过程，核心特性是语义相近的文本经过embedding后得到的向量也彼此接近。
created: '2026-08-26'
updated: '2026-08-26'
---

# Embedding

%% ytkb:def %%
embedding是将文本转换为向量的过程，核心特性是语义相近的文本经过embedding后得到的向量也彼此接近。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 语义相近的句子（如“马克喜欢吃水果”与“马克爱吃水果”）经过embedding后对应向量距离很近，而语义无关的句子（如“天气真好”）对应向量距离较远。（[06:00](https://youtu.be/WWdlme1EAGI?t=360)）
- Embedding 的作用是把每一个片段的文本转换为对应的向量。（[03:00](https://youtu.be/WWdlme1EAGI?t=180)）
%% ytkb:end %%

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 向量数据库通过 embedding 把每个词或每段文字转换成高维数字向量，本质是把文本内容『数字化』，类似照片被数字化存储后即可通过计算相似度进行搜索。（[03:00](https://youtu.be/CyLYY_xb5bQ?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rag-indexing]]
- [[vector]]
- [[vector-database]]
- [[vector-similarity]]
%% ytkb:end %%
