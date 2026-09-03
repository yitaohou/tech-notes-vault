---
title: Inverted Index
aliases: []
tags:
- concept
summary: 对文本块分词后记录每个词项出现在哪些文本块中的索引结构，用于支持关键词检索。
created: '2026-09-02'
updated: '2026-09-02'
---

# Inverted Index

%% ytkb:def %%
对文本块分词后记录每个词项出现在哪些文本块中的索引结构，用于支持关键词检索。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-data-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:ky7_1K3wfAY %%
### 来自 [[2026-08-26-agent搜索和记忆的基础设施腾讯云-elastichsearch-service-企业版详细攻略]]
- 倒排索引通过对文本分词并记录词项出现位置，使关键词搜索时能直接定位到包含该词的原文段落，是 Elasticsearch 第一阶段关键词搜索的核心技术。（[00:00](https://youtu.be/ky7_1K3wfAY?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[elasticsearch]]
- [[term-based-retrieval]]
%% ytkb:end %%
