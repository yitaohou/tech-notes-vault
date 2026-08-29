---
title: Dot Product Similarity
aliases: []
tags:
- concept
summary: 通过计算两个向量的点积（dot product）来衡量相似程度的方法，是目前较流行的向量相似度计算方案之一。
created: '2026-08-26'
updated: '2026-08-26'
---

# Dot Product Similarity

%% ytkb:def %%
通过计算两个向量的点积（dot product）来衡量相似程度的方法，是目前较流行的向量相似度计算方案之一。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 目前比较流行的向量相似度计算方案除了余弦相似度和欧式距离外，还包括点积（dot product）。（[09:03](https://youtu.be/WWdlme1EAGI?t=543)）
- 点积的计算方法是：先从向量A向向量B作垂线得到投影距离，再将该投影距离与向量B的长度相乘，乘积越大代表两个向量相似度越高。（[12:03](https://youtu.be/WWdlme1EAGI?t=723)）
- 两个向量方向一致时点积为正且随向量长度增大而增大；方向相反时点积为负；两向量垂直时点积为0，据此可判断向量方向的一致程度。（[12:03](https://youtu.be/WWdlme1EAGI?t=723)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cosine-similarity]]
- [[euclidean-distance]]
- [[vector-similarity]]
- [[vector-similarity-calculation]]
%% ytkb:end %%
