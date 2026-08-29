---
title: GraphQL Origin Motivation
aliases: []
tags:
- concept
summary: Facebook 创建 GraphQL 是为了解决客户端需要对多个 REST API 分别发起请求、却依然拿不到确切所需数据这一痛点。
created: '2026-08-26'
updated: '2026-08-26'
---

# GraphQL Origin Motivation

%% ytkb:def %%
Facebook 创建 GraphQL 是为了解决客户端需要对多个 REST API 分别发起请求、却依然拿不到确切所需数据这一痛点。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- GraphQL 由 Facebook 发明，用于解决客户端对多个 REST API（如 user、post、comments、likes）分别请求却仍需多次调用才能拼齐所需数据的问题，这会累积增加页面整体延迟。（[78:18](https://youtu.be/oYxTTirKY8M?t=4698)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[graphql]]
- [[over-fetching-under-fetching]]
%% ytkb:end %%
