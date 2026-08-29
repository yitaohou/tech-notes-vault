---
title: GraphQL
aliases: []
tags:
- concept
summary: 一种适合用来构建 backend for frontend 的查询技术，可让客户端按需精确获取所需数据。
created: '2026-08-26'
updated: '2026-08-26'
---

# GraphQL

%% ytkb:def %%
一种适合用来构建 backend for frontend 的查询技术，可让客户端按需精确获取所需数据。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- GraphQL 被认为是构建 backend for frontend 的优秀技术选择之一。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- GraphQL 只提供一个单一端点（single endpoint）处理所有操作，客户端通过请求中的 payload 精确指定自己想要获取的数据字段。（[33:05](https://youtu.be/oYxTTirKY8M?t=1985)）
- GraphQL API 同样以 HTTP 作为底层协议，而不是 WebSocket 或 gRPC。（[41:50](https://youtu.be/oYxTTirKY8M?t=2510)）
- GraphQL 通过让客户端精确声明自己所需的字段，解决了传统 REST API 常见的 over-fetching（返回数据过多）或 under-fetching（返回数据不足、需多次请求拼凑数据）问题。（[77:05](https://youtu.be/oYxTTirKY8M?t=4625)）
- GraphQL 只暴露单一端点处理所有数据交互，请求本质仍是 HTTP 请求，但客户端可在请求中指定响应的精确形状（shape），例如只取 user 的 name、posts 的 title，从而避免 over-fetching。（[78:18](https://youtu.be/oYxTTirKY8M?t=4698)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-protocol-design-influence]]
- [[backend-for-frontend]]
- [[graphql-operation-types]]
- [[graphql-schema-contract]]
- [[over-fetching-under-fetching]]
- [[restful-api-design]]
%% ytkb:end %%
