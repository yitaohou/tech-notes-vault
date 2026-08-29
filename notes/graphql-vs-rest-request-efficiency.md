---
title: GraphQL vs REST Request Efficiency
aliases: []
tags:
- concept
summary: 对于跨多个资源的数据需求，GraphQL 可用单次请求完成，而 REST 通常需要发起多次独立请求。
created: '2026-08-26'
updated: '2026-08-26'
---

# GraphQL vs REST Request Efficiency

%% ytkb:def %%
对于跨多个资源的数据需求，GraphQL 可用单次请求完成，而 REST 通常需要发起多次独立请求。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 对于同一份跨用户、帖子、关注者等多个资源的数据需求，GraphQL 可以用一次请求完成，而 RESTful API 通常需要发起三次独立请求。（[37:10](https://youtu.be/oYxTTirKY8M?t=2230)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[graphql]]
- [[over-fetching-under-fetching]]
%% ytkb:end %%
