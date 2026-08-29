---
title: GraphQL Mutation
aliases: []
tags:
- concept
summary: GraphQL 中用于修改数据的操作类型，相当于 RESTful API 中的 POST、PUT、PATCH、DELETE 方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# GraphQL Mutation

%% ytkb:def %%
GraphQL 中用于修改数据的操作类型，相当于 RESTful API 中的 POST、PUT、PATCH、DELETE 方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 任何对数据库进行写操作（如 createUser）的 GraphQL 请求都通过 mutation 完成，mutation 同样需要定义输入参数和返回类型。（[78:18](https://youtu.be/oYxTTirKY8M?t=4698)）
- GraphQL mutation 用于执行写操作（如 create post），调用时既传入要写入的字段（如 title、body），也指定写入完成后要返回的字段（如 ID、title）。（[81:20](https://youtu.be/oYxTTirKY8M?t=4880)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[graphql]]
- [[graphql-query]]
- [[graphql-schema-contract]]
%% ytkb:end %%
