---
title: UDP (User Datagram Protocol)
aliases: []
tags:
- concept
summary: 一种传输层协议，传输快速轻量，但不保证数据包一定送达，也没有握手或连接追踪机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# UDP (User Datagram Protocol)

%% ytkb:def %%
一种传输层协议，传输快速轻量，但不保证数据包一定送达，也没有握手或连接追踪机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-networking-protocols]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- UDP 不保证所有数据包都能送达，例如发送四个数据包，其中一个丢失后不会被重新推送给客户端，UDP 本身不会确保它最终被送达。（[60:11](https://youtu.be/oYxTTirKY8M?t=3611)）
- UDP 没有握手、连接建立或任何形式的追踪机制，因此传输开销更小、速度更快。（[60:11](https://youtu.be/oYxTTirKY8M?t=3611)）
- UDP 是 TCP 的更快但不可靠版本，二者都属于传输层协议，但实现数据传输的方式完全不同。（[57:11](https://youtu.be/oYxTTirKY8M?t=3431)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[tcp-protocol]]
- [[tcp-three-way-handshake]]
- [[transport-layer-tcp-udp]]
%% ytkb:end %%
