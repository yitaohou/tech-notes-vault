---
title: Term-based Retrieval (Lexical Retrieval)
aliases: []
tags:
- concept
summary: 也称为 lexical retrieval，一种基于关键词匹配来判断文档与查询相关性的检索方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Term-based Retrieval (Lexical Retrieval)

%% ytkb:def %%
也称为 lexical retrieval，一种基于关键词匹配来判断文档与查询相关性的检索方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- term-based retrieval（又称 lexical retrieval）通过关键词匹配来查找相关文档，做法简单直接，但存在明显局限。（[30:02](https://youtu.be/JV3pL1_mn2M?t=1802)）
- term-based retrieval 的局限之一：一篇文档可能包含某个关键词，但文档实际内容并不是围绕这个词展开的。（[30:02](https://youtu.be/JV3pL1_mn2M?t=1802)）
- 查询语句中往往包含很多词，但这些词的重要程度并不相同，term-based retrieval 难以区分词语的重要性差异。（[30:02](https://youtu.be/JV3pL1_mn2M?t=1802)）
- 简单的分词（tokenization）会丢失词语之间的语义关系，是 term-based retrieval 的另一个局限。（[30:02](https://youtu.be/JV3pL1_mn2M?t=1802)）
- term-based retrieval 在索引和查询阶段通常都比 embedding-based retrieval 更快，且能开箱即用地兼容 Elasticsearch 等现有系统。（[33:02](https://youtu.be/JV3pL1_mn2M?t=1982)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[embedding-based-retrieval]]
- [[hybrid-retrieval-pipeline]]
- [[tf-idf]]
%% ytkb:end %%
