---
title: AMQP
aliases: []
tags:
- concept
summary: AMQP（Advanced Message Queuing Protocol）是一种支持异步通信的消息协议，通过在 consumer 和 producer
  之间加入 message queue 实现解耦。
created: '2026-08-26'
updated: '2026-08-26'
---

# AMQP

%% ytkb:def %%
AMQP（Advanced Message Queuing Protocol）是一种支持异步通信的消息协议，通过在 consumer 和 producer 之间加入 message queue 实现解耦。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-messaging-queues]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- AMQP 允许在 consumer 和 producer 之间加入 message queue，从而实现异步通信（asynchronous communication）。（[57:11](https://youtu.be/oYxTTirKY8M?t=3431)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[message-broker-necessity]]
- [[message-broker-pub-sub]]
%% ytkb:end %%
