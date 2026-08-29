---
title: GraphQL Application-Level Caching
aliases: []
tags:
- concept
summary: 由于 GraphQL 使用单一端点，无法直接复用 HTTP caching，因此需要在应用层实现缓存策略。
created: '2026-08-26'
updated: '2026-08-26'
---

# GraphQL Application-Level Caching

%% ytkb:def %%
由于 GraphQL 使用单一端点，无法直接复用 HTTP caching，因此需要在应用层实现缓存策略。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 由于 GraphQL 使用单一端点，无法像 REST 那样直接利用 HTTP caching，因此需要采用 application-level caching。（[37:40](https://youtu.be/oYxTTirKY8M?t=2260)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[graphql]]
- [[rest-http-caching-headers]]
%% ytkb:end %%
