---
title: GraphQL Round-Trip Reduction
aliases: []
tags:
- concept
summary: GraphQL 允许客户端通过单次请求获取原本需要多次 REST 请求才能拿到的关联数据，从而减少网络往返次数（round trip）的优势。
created: '2026-08-26'
updated: '2026-08-26'
---

# GraphQL Round-Trip Reduction

%% ytkb:def %%
GraphQL 允许客户端通过单次请求获取原本需要多次 REST 请求才能拿到的关联数据，从而减少网络往返次数（round trip）的优势。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 在 RESTful API 中可能需要三次独立请求才能获取的关联数据，用 GraphQL 只需一次请求即可全部拿到，从而避免了不必要的多次往返。（[33:05](https://youtu.be/oYxTTirKY8M?t=1985)）
- 正因为能够减少 round trip，GraphQL 是构建复杂 UI（例如同一应用不同页面各自需要不同甚至嵌套数据结构）时相较 RESTful API 更推荐的选择。（[33:05](https://youtu.be/oYxTTirKY8M?t=1985)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[graphql]]
- [[over-fetching-under-fetching]]
- [[restful-api-design]]
%% ytkb:end %%
