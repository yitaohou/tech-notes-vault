---
title: GraphQL Query
aliases: []
tags:
- concept
summary: GraphQL 中用于读取数据的操作类型，相当于 RESTful API 中的 GET 请求。
created: '2026-08-26'
updated: '2026-08-26'
---

# GraphQL Query

%% ytkb:def %%
GraphQL 中用于读取数据的操作类型，相当于 RESTful API 中的 GET 请求。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- GraphQL query 需要声明函数名、输入参数（如 user ID）和返回类型（如返回 schema 中定义的 User 类型），是 GraphQL 读取数据的标准方式。（[78:18](https://youtu.be/oYxTTirKY8M?t=4698)）
- GraphQL 的 query 类似 REST API 中的 GET 请求，客户端可以精确指定需要哪些字段，例如从 user 中只取 name 和 posts 里的 title，服务端只返回这些精确匹配的数据。（[81:20](https://youtu.be/oYxTTirKY8M?t=4880)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[graphql]]
- [[graphql-mutation]]
- [[graphql-schema-contract]]
- [[restful-api-design]]
%% ytkb:end %%
