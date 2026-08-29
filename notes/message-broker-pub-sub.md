---
title: Message Broker / Pub-Sub System
aliases: []
tags:
- concept
summary: 如 Kafka、RabbitMQ 这类消息代理，作为发布订阅系统接收消息并负责将其分发给下游多个服务。
created: '2026-08-26'
updated: '2026-08-26'
---

# Message Broker / Pub-Sub System

%% ytkb:def %%
如 Kafka、RabbitMQ 这类消息代理，作为发布订阅系统接收消息并负责将其分发给下游多个服务。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-messaging-queues]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 为实现服务间解耦，需要引入一个 broker（如 Kafka 或 RabbitMQ）作为 pub/sub 系统，上游只需把消息发给 broker，由 broker 负责分发给各个下游服务。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[object-storage-upload-event-trigger]]
- [[service-to-service-decoupling-via-broker]]
%% ytkb:end %%
