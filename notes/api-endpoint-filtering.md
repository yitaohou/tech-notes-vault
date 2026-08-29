---
title: Filtering Support in List Endpoints
aliases: []
tags:
- concept
summary: 在返回列表数据的 API 接口中额外提供过滤参数，使客户端可按条件筛选结果子集的设计方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Filtering Support in List Endpoints

%% ytkb:def %%
在返回列表数据的 API 接口中额外提供过滤参数，使客户端可按条件筛选结果子集的设计方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 获取题目列表的接口除了分页参数外，还被设计为支持对题目集合进行过滤（filtering）。（[13:10](https://youtu.be/QBHTbtWSECg?t=790)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 真实场景中很少一次性返回全部结果，因此常通过查询参数（如 category、in_stock=true）对集合类接口的返回结果进行过滤。（[63:13](https://youtu.be/oYxTTirKY8M?t=3793)）
- 好的 REST API 应支持 filtering，允许客户端通过参数按条件筛选资源子集，而不是只能拿到全部数据。（[75:55](https://youtu.be/oYxTTirKY8M?t=4555)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[pagination-api-design]]
- [[restful-api-design]]
%% ytkb:end %%
