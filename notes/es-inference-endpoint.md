---
title: ES Inference Endpoint
aliases: []
tags:
- concept
summary: 在ES中通过DSL创建的推理端点，用于对接外部向量化服务，供索引写入和查询时调用完成文本向量化。
created: '2026-09-02'
updated: '2026-09-02'
---

# ES Inference Endpoint

%% ytkb:def %%
在ES中通过DSL创建的推理端点，用于对接外部向量化服务，供索引写入和查询时调用完成文本向量化。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:ky7_1K3wfAY %%
### 来自 [[2026-08-26-agent搜索和记忆的基础设施腾讯云-elastichsearch-service-企业版详细攻略]]
- 复制官方提供的创建推理端点DSL，在Kibana控制台粘贴并将其中的URL与API key替换为推理服务的实际值后执行，即可在ES集群中创建一个对接外部推理服务的推理端点。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[embedding-model-integration-methods-es]]
- [[es-inference-service-api-key]]
- [[es-ingest-pipeline-auto-embedding]]
%% ytkb:end %%
