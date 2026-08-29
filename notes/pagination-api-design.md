---
title: Pagination in API Design
aliases: []
tags:
- concept
summary: 通过 page 和 limit 等查询参数控制列表类接口单次返回结果数量的 API 设计技术，用于避免一次性返回过多数据。
created: '2026-08-26'
updated: '2026-08-26'
---

# Pagination in API Design

%% ytkb:def %%
通过 page 和 limit 等查询参数控制列表类接口单次返回结果数量的 API 设计技术，用于避免一次性返回过多数据。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 获取题目列表的 GET /problems 接口设计为支持分页，默认 page=1、limit=100，即首次请求返回前 100 道题目。（[13:40](https://youtu.be/QBHTbtWSECg?t=820)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 当数据量很大（如成千上万篇帖子）时，API 应通过带 limit 和 offset 的分页返回结果，而不是一次性返回所有数据。（[40:20](https://youtu.be/oYxTTirKY8M?t=2420)）
- 分页通过 page 和 limit 两个 query parameter 实现：page 指定要获取第几页，limit 限制每页返回的条目数（即前端实际要展示的数量）；如果不传 limit，会返回从该页开始的所有剩余数据，条目数可能非常多。（[1:06:15](https://youtu.be/oYxTTirKY8M?t=3975)）
- 在 page-based pagination 中，用户点击下一页时前端会发起新的请求（如 page 参数变为3），从服务端获取下一批数据。（[1:06:15](https://youtu.be/oYxTTirKY8M?t=3975)）
- 分页设计不能只提供页码参数，还需要提供 limit 参数来控制每页返回的资源数量，否则客户端无法控制单次获取的数据量。（[76:05](https://youtu.be/oYxTTirKY8M?t=4565)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-endpoint-filtering]]
- [[api-payload-minimization]]
- [[cursor-based-pagination]]
- [[offset-based-pagination]]
- [[restful-api-design]]
%% ytkb:end %%
