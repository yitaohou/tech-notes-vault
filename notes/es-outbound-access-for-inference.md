---
title: ES Node Outbound Access for External Inference
aliases: []
tags:
- concept
summary: 在ES集群管理设置中开启的节点出站访问开关，用于允许集群机器主动访问外部的推理服务。
created: '2026-09-02'
updated: '2026-09-02'
---

# ES Node Outbound Access for External Inference

%% ytkb:def %%
在ES集群管理设置中开启的节点出站访问开关，用于允许集群机器主动访问外部的推理服务。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:ky7_1K3wfAY %%
### 来自 [[2026-08-26-agent搜索和记忆的基础设施腾讯云-elastichsearch-service-企业版详细攻略]]
- 要让ES集群使用腾讯云的原子化推理服务，需要先在集群管理的更多设置中打开节点出站访问的开关，允许集群机器访问外部推理服务。（[06:01](https://youtu.be/ky7_1K3wfAY?t=361)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[embedding-model-integration-methods-es]]
%% ytkb:end %%
