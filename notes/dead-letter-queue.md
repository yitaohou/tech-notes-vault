---
title: Dead Letter Queue
aliases: []
tags:
- concept
summary: 消息经过多次重试仍未成功投递后被转移进入的专门队列，用于统一存放这类失败消息。
created: '2026-08-26'
updated: '2026-08-26'
---

# Dead Letter Queue

%% ytkb:def %%
消息经过多次重试仍未成功投递后被转移进入的专门队列，用于统一存放这类失败消息。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-messaging-queues]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 如果消息始终无法被投递成功，会被放入一个专门的队列，通常称为 dead letter queue（消息的墓地）。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dead-letter-queue-alerting]]
- [[message-redelivery-mechanism]]
%% ytkb:end %%
