---
title: Long Polling Scalability Limit
aliases: []
tags:
- concept
summary: 客户端轮询（polling）方式实现简单、健壮性强，但大量客户端同时反复请求会对后端造成持续压力，扩展性较差的问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# Long Polling Scalability Limit

%% ytkb:def %%
客户端轮询（polling）方式实现简单、健壮性强，但大量客户端同时反复请求会对后端造成持续压力，扩展性较差的问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 轮询方式虽然易于实现且很健壮，但如果有上万个客户端同时轮询，请求量会成倍叠加，容易把后端打垮，本质上是自己对自己发起了DDOS，因此扩展性不好。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[server-sent-events-llm]]
- [[websocket-communication]]
%% ytkb:end %%
