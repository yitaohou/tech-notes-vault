---
title: GraphQL Operation Types
aliases: []
tags:
- concept
summary: GraphQL 中区分不同操作意图的三种类型：读取数据用 query，更新数据用 mutation，实时通信用 subscription。
created: '2026-08-26'
updated: '2026-08-26'
---

# GraphQL Operation Types

%% ytkb:def %%
GraphQL 中区分不同操作意图的三种类型：读取数据用 query，更新数据用 mutation，实时通信用 subscription。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- GraphQL 用 query 表示数据读取操作，用 mutation 表示数据更新操作（相当于 RESTful 中的 put、patch 或 post），并额外提供 subscription 操作用于实时通信。（[33:05](https://youtu.be/oYxTTirKY8M?t=1985)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[graphql]]
- [[real-time-communication-alternatives]]
%% ytkb:end %%
