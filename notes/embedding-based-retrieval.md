---
title: Embedding-Based Retrieval
aliases: []
tags:
- concept
summary: 在语义层面而非词汇层面计算相关性的检索方法，根据文档语义与查询语义的接近程度对文档排序。
created: '2026-08-26'
updated: '2026-09-02'
---

# Embedding-Based Retrieval

%% ytkb:def %%
在语义层面而非词汇层面计算相关性的检索方法，根据文档语义与查询语义的接近程度对文档排序。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- embedding-based retrieval 长期来看往往能显著优于 term-based retrieval，尤其是在对 embedding 模型和检索器做过 fine-tune 的情况下。（[33:02](https://youtu.be/JV3pL1_mn2M?t=1982)）
- embedding-based retrieval 的缺点在于难以精确检索特定人名或错误代码这类需要精确匹配的内容，且生成 embedding 本身可能带来额外成本和延迟。（[33:02](https://youtu.be/JV3pL1_mn2M?t=1982)）
%% ytkb:end %%

%% ytkb:video:ky7_1K3wfAY %%
### 来自 [[2026-08-26-agent搜索和记忆的基础设施腾讯云-elastichsearch-service-企业版详细攻略]]
- Elasticsearch 的语义搜索阶段会先用嵌入模型对文本块做向量化，检索时把用户问题同样向量化并计算向量相似度，从而在问题与原文没有相同关键词时依然能找到语义最相近的内容。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[elasticsearch]]
- [[embedding]]
- [[embedding-model]]
- [[rag-retrieval]]
- [[term-based-retrieval]]
- [[vector-similarity]]
%% ytkb:end %%
