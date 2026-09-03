---
title: Hybrid Retrieval Pipeline
aliases: []
tags:
- concept
summary: 生产环境中常见的检索架构：先用成本较低、精度较弱的检索器（如 term-based search）召回候选，再用精度更高但更昂贵的方法（如 KNN）在候选中精选最佳结果。
created: '2026-08-26'
updated: '2026-09-02'
---

# Hybrid Retrieval Pipeline

%% ytkb:def %%
生产环境中常见的检索架构：先用成本较低、精度较弱的检索器（如 term-based search）召回候选，再用精度更高但更昂贵的方法（如 KNN）在候选中精选最佳结果。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 生产级检索系统通常组合多种检索方式，例如先用便宜的 term-based search 拿到候选集，再用更精确但更贵的 KNN 从候选中筛出最佳结果。（[33:02](https://youtu.be/JV3pL1_mn2M?t=1982)）
%% ytkb:end %%

%% ytkb:video:ky7_1K3wfAY %%
### 来自 [[2026-08-26-agent搜索和记忆的基础设施腾讯云-elastichsearch-service-企业版详细攻略]]
- 腾讯云 Elasticsearch Service 企业版通过混合检索（hybrid retrieval）与重排序（rerank）来提高 RAG 系统的召回质量。（[09:02](https://youtu.be/ky7_1K3wfAY?t=542)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[approximate-nearest-neighbor-search]]
- [[cross-encoder-rerank]]
- [[embedding-based-retrieval]]
- [[rag-rerank]]
- [[term-based-retrieval]]
%% ytkb:end %%
