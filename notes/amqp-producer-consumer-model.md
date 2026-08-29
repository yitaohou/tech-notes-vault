---
title: AMQP Producer-Consumer Model
aliases: []
tags:
- concept
summary: AMQP 架构中生产者将消息发布给 broker、消费者再从 broker 的队列中获取消息处理的角色划分方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# AMQP Producer-Consumer Model

%% ytkb:def %%
AMQP 架构中生产者将消息发布给 broker、消费者再从 broker 的队列中获取消息处理的角色划分方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-messaging-queues]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 在 AMQP 中，producer（例如 web service 或支付系统）把消息发布到 message broker，broker 内部维护 queue，consumer（例如支付处理器或通知系统）再从队列中取出消息进行处理。（[51:09](https://youtu.be/oYxTTirKY8M?t=3069)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[amqp]]
- [[message-broker-pub-sub]]
%% ytkb:end %%
