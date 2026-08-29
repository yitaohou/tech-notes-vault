---
title: Attention Score Computation
aliases: []
tags:
- concept
summary: 模型通过比较 query 向量和 key 向量的相似度来决定给每个输入 token 分配多少注意力的过程。
created: '2026-08-26'
updated: '2026-08-26'
---

# Attention Score Computation

%% ytkb:def %%
模型通过比较 query 向量和 key 向量的相似度来决定给每个输入 token 分配多少注意力的过程。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-llm-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 模型通过比较 Q 向量和 K 向量的相似度来决定给每个输入 token 分配多少注意力，相似度越高，该 token 对应的 V 向量对输出的影响就越大。（[03:00](https://youtu.be/JV3pL1_mn2M?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[long-context-computational-cost]]
- [[query-key-value-vectors]]
%% ytkb:end %%
