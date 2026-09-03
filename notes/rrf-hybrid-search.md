---
title: RRF Hybrid Search
aliases: []
tags:
- concept
summary: Reciprocal Rank Fusion（RRF）混合检索是同时执行关键词匹配和向量语意检索两路查询、再用RRF算法把两路结果按排名融合排序的检索方法。
created: '2026-09-02'
updated: '2026-09-02'
---

# RRF Hybrid Search

%% ytkb:def %%
Reciprocal Rank Fusion（RRF）混合检索是同时执行关键词匹配和向量语意检索两路查询、再用RRF算法把两路结果按排名融合排序的检索方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:ky7_1K3wfAY %%
### 来自 [[2026-08-26-agent搜索和记忆的基础设施腾讯云-elastichsearch-service-企业版详细攻略]]
- RRF混合检索会同时执行两路查询——第一路做传统关键词匹配，第二路根据向量索引做语意检索，最终ES通过RRF算法把两路结果综合排序，返回最相关的几个文本块。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[diskbbq-vector-index]]
- [[embedding-based-retrieval]]
- [[hybrid-retrieval-pipeline]]
- [[term-based-retrieval]]
%% ytkb:end %%
