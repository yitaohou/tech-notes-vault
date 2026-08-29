---
title: Message Redelivery Mechanism
aliases: []
tags:
- concept
summary: 消息代理提供的重投递功能：若消费方未在规定时间内确认（ack）收到消息，broker 会在一段时间后重新投递该消息。
created: '2026-08-26'
updated: '2026-08-26'
---

# Message Redelivery Mechanism

%% ytkb:def %%
消息代理提供的重投递功能：若消费方未在规定时间内确认（ack）收到消息，broker 会在一段时间后重新投递该消息。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- broker 具备 redelivery（重投）功能：消费服务（如 file service）需要 acknowledge 收到消息，若未确认，broker 会在一定时间后重新投递该消息。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dead-letter-queue]]
- [[message-broker-high-availability]]
%% ytkb:end %%
