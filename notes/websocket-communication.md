---
title: WebSocket Communication
aliases: []
tags:
- concept
summary: WebSocket 是一种在客户端与服务端之间建立双向通信通道的协议，允许双方随时互相主动发送消息。
created: '2026-08-26'
updated: '2026-08-26'
---

# WebSocket Communication

%% ytkb:def %%
WebSocket 是一种在客户端与服务端之间建立双向通信通道的协议，允许双方随时互相主动发送消息。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- WebSocket 让每个客户端与后端建立一条双向通信通道，消息可以双向实时推送，非常适合聊天类应用中点对点即时通讯的场景。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
- WebSocket 对后端而言计算开销较大、扩展性不好，且实现复杂度也比轮询和SSE更高。（[48:09](https://youtu.be/AMerB8XjfZ0?t=2889)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- WebSocket 非常适合双向通信场景，例如聊天应用中客户端和服务端都需要不断发送消息片段，但代价是 overhead 较大，且对服务端资源消耗很高，多数场景并不需要。（[36:09](https://youtu.be/KuClyhvSzXk?t=2169)）
- 相较于 polling，WebSocket 通过在客户端与服务端之间打开一条持续的双向通信通道，是实现实时通信的下一个替代方案。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- WebSocket 支持双向实时通信，适合聊天应用、视频流等需要实时数据交互的场景。（[41:40](https://youtu.be/oYxTTirKY8M?t=2500)）
- WebSocket 是用于实现实时通信的一种常见应用层协议类型。（[45:08](https://youtu.be/oYxTTirKY8M?t=2708)）
- 在 WebSocket 建立连接后，通信是双向的：客户端仍可以主动发起请求获取额外数据，服务端也能独立推送数据，因此相比轮询大幅减少了不必要的请求带来的带宽消耗。（[51:09](https://youtu.be/oYxTTirKY8M?t=3069)）
- WebSocket 是应用层中用于实现实时通信（real-time communication）的协议之一，与 AMQP、gRPC 并列。（[57:11](https://youtu.be/oYxTTirKY8M?t=3431)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[amqp-protocol]]
- [[api-protocol-design-influence]]
- [[application-layer-protocol]]
- [[grpc-protocol]]
- [[llm-response-communication-asymmetry]]
- [[long-polling-scalability-limit]]
- [[polling-technique]]
- [[server-sent-events-llm]]
- [[websocket-server-push]]
%% ytkb:end %%
