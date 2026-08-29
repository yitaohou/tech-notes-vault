---
title: Vector Similarity Calculation
aliases: []
tags:
- concept
summary: 向量数据库判断片段与用户问题相关程度所用的计算过程，即把两个向量代入相似度公式得出一个相似度数值。
created: '2026-08-26'
updated: '2026-08-26'
---

# Vector Similarity Calculation

%% ytkb:def %%
向量数据库判断片段与用户问题相关程度所用的计算过程，即把两个向量代入相似度公式得出一个相似度数值。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 计算向量相似度时，相似度公式的第一个参数固定为用户问题对应的向量，第二个参数则是待比较的片段向量；对所有片段逐一计算后排序，取相似度最高的若干个。（[09:03](https://youtu.be/WWdlme1EAGI?t=543)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cosine-similarity]]
- [[dot-product-similarity]]
- [[euclidean-distance]]
- [[top-k-retrieval]]
%% ytkb:end %%
