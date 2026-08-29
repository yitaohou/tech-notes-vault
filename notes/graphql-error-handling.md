---
title: GraphQL Error Handling
aliases: []
tags:
- concept
summary: GraphQL API 无论请求是否出错都统一返回 HTTP 200 状态码，真正的错误信息通过响应体中的 errors 字段单独表达。
created: '2026-08-26'
updated: '2026-08-26'
---

# GraphQL Error Handling

%% ytkb:def %%
GraphQL API 无论请求是否出错都统一返回 HTTP 200 状态码，真正的错误信息通过响应体中的 errors 字段单独表达。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- GraphQL API 无论是否出错都始终返回 200 OK 状态码，因此错误必须通过响应体中的 errors 字段表示，并可在 errors 中携带具体的状态码（如 404）和错误信息。（[81:20](https://youtu.be/oYxTTirKY8M?t=4880)）
- GraphQL 允许在同一响应中同时返回部分正确数据与 errors 字段，例如某个字段（如 user）为 null，同时 errors 中说明该字段查询失败的状态码、消息和路径。（[81:20](https://youtu.be/oYxTTirKY8M?t=4880)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[graphql]]
- [[restful-api-design]]
%% ytkb:end %%
