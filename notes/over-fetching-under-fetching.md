---
title: Over-fetching / Under-fetching
aliases: []
tags:
- concept
summary: 当单一 API 试图同时满足数据需求差异很大的多个客户端时，出现的数据过多（over-fetching）或数据不足、需多次请求（under-fetching）的问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# Over-fetching / Under-fetching

%% ytkb:def %%
当单一 API 试图同时满足数据需求差异很大的多个客户端时，出现的数据过多（over-fetching）或数据不足、需多次请求（under-fetching）的问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-graphql]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 如果把 desktop 和 mobile 的数据需求都塞进同一个 API：接口做大会导致 mobile 端 over-fetch 到不需要的数据，接口做小又会导致 desktop 端需要多次请求才能拿到同样的数据，即 under-fetching。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- REST 采用资源导向（resource-based）的端点设计（如 users、followers、posts 各自独立端点），因此获取像用户详情、帖子、关注者这类关联数据时，通常需要分别发起多次请求才能拿到全部所需数据。（[33:05](https://youtu.be/oYxTTirKY8M?t=1985)）
- GraphQL 允许在嵌套对象（如 comments）内部也精确指定所需字段，从而在任意嵌套层级都能避免 over-fetching，这是它区别于 RESTful API 固定响应结构的关键优势。（[78:18](https://youtu.be/oYxTTirKY8M?t=4698)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[backend-for-frontend]]
- [[graphql]]
- [[graphql-round-trip-reduction]]
- [[restful-api-design]]
%% ytkb:end %%
