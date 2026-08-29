---
title: Message Broker High Availability
aliases: []
tags:
- concept
summary: 消息代理（broker）作为微服务间通信的中介，需要被设计为高可用，确保持续在线且不丢失消息。
created: '2026-08-26'
updated: '2026-08-26'
---

# Message Broker High Availability

%% ytkb:def %%
消息代理（broker）作为微服务间通信的中介，需要被设计为高可用，确保持续在线且不丢失消息。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- message broker 需要被设计为 highly available，核心目标是保持稳定运行且不丢失（crush）消息。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[distributed-architecture-avoid-spof]]
- [[message-queue-load-smoothing]]
%% ytkb:end %%
