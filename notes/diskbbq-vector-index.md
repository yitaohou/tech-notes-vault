---
title: DiskBBQ Vector Index
aliases: []
tags:
- concept
summary: ES中一种把向量数据存储到磁盘而非全部载入内存的向量索引方案，用于大幅降低大规模向量搜索的内存成本。
created: '2026-09-02'
updated: '2026-09-02'
---

# DiskBBQ Vector Index

%% ytkb:def %%
ES中一种把向量数据存储到磁盘而非全部载入内存的向量索引方案，用于大幅降低大规模向量搜索的内存成本。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:ky7_1K3wfAY %%
### 来自 [[2026-08-26-agent搜索和记忆的基础设施腾讯云-elastichsearch-service-企业版详细攻略]]
- 创建索引时，文本字段使用传统倒排索引做关键词搜索，向量字段则使用DiskBBQ做语意检索，DiskBBQ可以把向量数据存储在磁盘上，避免把海量向量全部塞进内存，从而大幅降低大规模向量搜索的内存成本。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[embedding-based-retrieval]]
- [[vector-database]]
%% ytkb:end %%
