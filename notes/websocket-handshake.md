---
title: WebSocket Handshake
aliases: []
tags:
- concept
summary: WebSocket 通信建立时，客户端与服务端先通过一次 handshake 完成协议升级，此后双方即可在同一连接上进行双向通信。
created: '2026-08-26'
updated: '2026-08-26'
---

# WebSocket Handshake

%% ytkb:def %%
WebSocket 通信建立时，客户端与服务端先通过一次 handshake 完成协议升级，此后双方即可在同一连接上进行双向通信。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-networking]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- WebSocket 的 handshake 只发生在第一次请求，完成之后客户端与服务端之间就建立了持久的双向通信通道。（[51:09](https://youtu.be/oYxTTirKY8M?t=3069)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[websocket-communication]]
%% ytkb:end %%
