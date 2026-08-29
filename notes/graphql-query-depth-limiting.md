---
title: GraphQL Query Depth Limiting
aliases: []
tags:
- concept
summary: 为防止 GraphQL 查询因关联字段无限嵌套（如 user→post→comment→...）导致性能问题，限制查询可嵌套的最大层数的做法。
created: '2026-08-26'
updated: '2026-08-26'
---

# GraphQL Query Depth Limiting

%% ytkb:def %%
为防止 GraphQL 查询因关联字段无限嵌套（如 user→post→comment→...）导致性能问题，限制查询可嵌套的最大层数的做法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- GraphQL 查询可能出现无限嵌套（如 user 嵌套 post 再嵌套 comment），最佳实践是设置查询深度限制（如最多6到7层）来避免过深的嵌套查询。（[81:20](https://youtu.be/oYxTTirKY8M?t=4880)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[graphql]]
%% ytkb:end %%
