---
title: WebSocket Server Push
aliases: []
tags:
- concept
summary: 指 WebSocket handshake 完成后，服务端无需等待客户端请求即可主动将新数据推送给客户端的能力。
created: '2026-08-26'
updated: '2026-08-26'
---

# WebSocket Server Push

%% ytkb:def %%
指 WebSocket handshake 完成后，服务端无需等待客户端请求即可主动将新数据推送给客户端的能力。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- handshake 完成后，一旦服务端产生了新数据，它可以主动推送给客户端而不必等待客户端发起请求，从而实现最低延迟的实时数据更新。（[51:09](https://youtu.be/oYxTTirKY8M?t=3069)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[websocket-communication]]
- [[websocket-handshake]]
%% ytkb:end %%
