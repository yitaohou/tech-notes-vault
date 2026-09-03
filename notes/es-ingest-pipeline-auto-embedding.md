---
title: ES Ingest Pipeline for Automatic Embedding
aliases: []
tags:
- concept
summary: ES中配置的一种数据写入流水线，在数据写入索引时自动调用推理端点把文本字段转换为向量。
created: '2026-09-02'
updated: '2026-09-02'
---

# ES Ingest Pipeline for Automatic Embedding

%% ytkb:def %%
ES中配置的一种数据写入流水线，在数据写入索引时自动调用推理端点把文本字段转换为向量。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:ky7_1K3wfAY %%
### 来自 [[2026-08-26-agent搜索和记忆的基础设施腾讯云-elastichsearch-service-企业版详细攻略]]
- 创建ingest pipeline后，数据写入ES索引时会自动调用之前创建的推理端点对文本进行向量化，无需手动预先做embedding再写入。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[embedding]]
- [[es-inference-endpoint]]
%% ytkb:end %%
