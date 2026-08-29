---
title: Message Durability on Broker Crash
aliases: []
tags:
- concept
summary: 即使 message broker 本身崩溃，消息依然不会丢失的持久化保证，通常通过把消息存储在独立数据库实现。
created: '2026-08-26'
updated: '2026-08-26'
---

# Message Durability on Broker Crash

%% ytkb:def %%
即使 message broker 本身崩溃，消息依然不会丢失的持久化保证，通常通过把消息存储在独立数据库实现。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 即便 broker 崩溃，消息也要保证 durable（持久化），常见做法是把消息存储在一个单独的数据库中。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[message-broker-high-availability]]
%% ytkb:end %%
