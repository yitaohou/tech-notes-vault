---
title: Producer-Consumer Coupling Scalability Problem
aliases: []
tags:
- concept
summary: 若生产者服务需要显式知道并逐一调用所有下游消费者，随着消费者数量增加，生产者代码需要不断修改，导致系统难以扩展的问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# Producer-Consumer Coupling Scalability Problem

%% ytkb:def %%
若生产者服务需要显式知道并逐一调用所有下游消费者，随着消费者数量增加，生产者代码需要不断修改，导致系统难以扩展的问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-messaging-queues]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 如果不引入 broker，产生事件的服务就必须自己维护一份下游订阅者列表并逐个通知，这种硬编码的点对点通知方式不具备良好的可扩展性，新增订阅者就要改动生产者代码。（[33:08](https://youtu.be/Qa-7iWxDz1A?t=1988)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[event-fan-out-multiple-subscribers]]
- [[message-broker-necessity]]
%% ytkb:end %%
