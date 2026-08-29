---
title: TCP (Transmission Control Protocol)
aliases: []
tags:
- concept
summary: 一种传输层协议，通过三步握手建立连接，并保证数据包最终会被可靠送达，但相对 UDP 更慢、开销更大。
created: '2026-08-26'
updated: '2026-08-26'
---

# TCP (Transmission Control Protocol)

%% ytkb:def %%
一种传输层协议，通过三步握手建立连接，并保证数据包最终会被可靠送达，但相对 UDP 更慢、开销更大。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-networking-protocols]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- TCP 是比 UDP 更安全可靠但速度更慢的协议，需要先完成连接建立（握手）才能开始数据传输。（[60:11](https://youtu.be/oYxTTirKY8M?t=3611)）
- TCP 中若某个数据包丢失，会在超时后重新发送该数据包，从而保证所有数据最终都能被完整送达，这与 UDP 数据可能丢失但不重发形成对比。（[60:11](https://youtu.be/oYxTTirKY8M?t=3611)）
- TCP 保证所有数据包都能被送达，如果某个包丢失或乱序到达，TCP 会重新发送或重新排序该包，就像寄送带有回执、追踪和签收要求的包裹一样。（[57:11](https://youtu.be/oYxTTirKY8M?t=3431)）
- TCP 会对乱序到达的数据包进行重新排序，例如客户端依次收到第一、第三、第二个包时，TCP 会将其重排为第一、第二、第三的正确顺序。（[57:11](https://youtu.be/oYxTTirKY8M?t=3431)）
- TCP 的可靠性机制（确认、重传、重排序）会带来额外开销（overhead），因此涉及支付、身份验证或用户数据的 API 通常选择使用 TCP。（[57:11](https://youtu.be/oYxTTirKY8M?t=3431)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authentication-service-login-flow]]
- [[tcp-three-way-handshake]]
- [[transport-layer-tcp-udp]]
- [[udp-protocol]]
%% ytkb:end %%
