---
title: Embedding-Based Retrieval
aliases: []
tags:
- concept
summary: 在语义层面而非词汇层面计算相关性的检索方法，根据文档语义与查询语义的接近程度对文档排序。
created: '2026-08-26'
updated: '2026-08-26'
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

## 相关概念

%% ytkb:related %%
- [[embedding-model]]
- [[rag-retrieval]]
- [[term-based-retrieval]]
%% ytkb:end %%
