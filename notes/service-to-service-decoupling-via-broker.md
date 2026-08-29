---
title: Service-to-Service Decoupling via Broker
aliases: []
tags:
- concept
summary: 上游服务（如对象存储的事件触发源）只需知道并对接一个 broker/API，无需了解所有下游服务的存在，从而实现服务间解耦。
created: '2026-08-26'
updated: '2026-08-26'
---

# Service-to-Service Decoupling via Broker

%% ytkb:def %%
上游服务（如对象存储的事件触发源）只需知道并对接一个 broker/API，无需了解所有下游服务的存在，从而实现服务间解耦。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 对象存储不需要知道系统里有哪些下游服务，它只需把上传事件发给一个统一的 broker，由 broker 负责把消息分发给实时服务、通知服务等具体消费者，这才是现实可行的服务间通信方式。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[message-broker-pub-sub]]
- [[object-storage-upload-event-trigger]]
%% ytkb:end %%
