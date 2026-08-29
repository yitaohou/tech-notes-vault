---
title: GraphQL Schema Evolution Without Versioning
aliases: []
tags:
- concept
summary: GraphQL 的 schema 通常不采用整体版本号迭代的方式，而是可直接修改字段或对个别字段做增量版本化。
created: '2026-08-26'
updated: '2026-08-26'
---

# GraphQL Schema Evolution Without Versioning

%% ytkb:def %%
GraphQL 的 schema 通常不采用整体版本号迭代的方式，而是可直接修改字段或对个别字段做增量版本化。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- GraphQL 的 schema 通常不采用像 REST 那样的整体版本号（V1、V2）迭代方式，而是可以直接修改字段，或对个别字段做增量版本化（如新增 followersV2 字段）。（[37:24](https://youtu.be/oYxTTirKY8M?t=2244)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[graphql]]
- [[rest-api-explicit-versioning]]
%% ytkb:end %%
