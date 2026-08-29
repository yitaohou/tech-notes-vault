---
title: RAG 重排（Rerank）阶段
aliases: []
tags:
- concept
summary: 重排是 RAG 流程中紧接召回之后的精筛阶段，使用准确率更高但成本更高的方法（如 cross encoder）从召回结果中进一步挑选出最相关的少数片段。
created: '2026-08-26'
updated: '2026-08-26'
---

# RAG 重排（Rerank）阶段

%% ytkb:def %%
重排是 RAG 流程中紧接召回之后的精筛阶段，使用准确率更高但成本更高的方法（如 cross encoder）从召回结果中进一步挑选出最相关的少数片段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WWdlme1EAGI %%
### 来自 [[2025-06-21-rag-工作机制详解一个高质量知识库背后的技术全流程]]
- 重排阶段从召回阶段选出的10个片段中，再挑选出3个与用户问题最相似的片段，作为最终结果。（[12:03](https://youtu.be/WWdlme1EAGI?t=723)）
- 召回与重排分两个阶段进行，而不是在召回阶段直接选出3个片段，是因为两阶段使用的文本相似度计算逻辑不同，先粗筛再精排的组合效果优于单独使用召回直接选出3个的效果。（[12:03](https://youtu.be/WWdlme1EAGI?t=723)）
- 召回与重排的关系可类比公司招聘的简历筛选与面试环节：召回像是从海量简历中粗略挑出10份候选人，重排则像是对这10人逐一面试、精细判断，最终录用3人。（[12:03](https://youtu.be/WWdlme1EAGI?t=723)）
%% ytkb:end %%

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 当受限于 context window 需要减少检索到的文档数量时，对初始检索排序结果做进一步重排（rerank）尤其有用。（[33:02](https://youtu.be/JV3pL1_mn2M?t=1982)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cross-encoder]]
- [[cross-encoder-rerank]]
- [[rag-retrieval-recall]]
- [[recency-weighted-reranking]]
%% ytkb:end %%
