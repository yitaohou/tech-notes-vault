---
title: API Round-Trip Reduction
aliases: []
tags:
- concept
summary: 指通过在一次请求/响应中顺带携带后续会用到的数据，来减少客户端需要发起的额外请求次数的API设计取舍。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Round-Trip Reduction

%% ytkb:def %%
指通过在一次请求/响应中顺带携带后续会用到的数据，来减少客户端需要发起的额外请求次数的API设计取舍。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-api-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 如果明确知道客户端后续会用到某些数据，可以在当前请求的响应中顺带一起返回，以减少额外的请求往返（round trip），而不必为此单独新建一个接口。（[40:50](https://youtu.be/oYxTTirKY8M?t=2450)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-payload-minimization]]
%% ytkb:end %%
