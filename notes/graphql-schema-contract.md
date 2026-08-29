---
title: GraphQL Schema as Contract
aliases: []
tags:
- concept
summary: GraphQL schema 是客户端与服务器之间关于数据类型和可用操作的契约（contract）。
created: '2026-08-26'
updated: '2026-08-26'
---

# GraphQL Schema as Contract

%% ytkb:def %%
GraphQL schema 是客户端与服务器之间关于数据类型和可用操作的契约（contract）。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- GraphQL schema 中定义类型（type）及其全部字段，若字段本身不是原始类型（如 posts 是一个 Post 数组），则该类型可以单独在 schema 中再定义。（[78:18](https://youtu.be/oYxTTirKY8M?t=4698)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[graphql]]
- [[graphql-mutation]]
- [[graphql-query]]
%% ytkb:end %%
