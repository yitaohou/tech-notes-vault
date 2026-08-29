---
title: Message Broker Necessity
aliases: []
tags:
- concept
summary: 在生产者与消费者服务之间引入专门的中间层（broker），负责接收事件并高可靠、高持久性地投递给下游服务，避免直接同步调用带来的脆弱性。
created: '2026-08-26'
updated: '2026-08-26'
---

# Message Broker Necessity

%% ytkb:def %%
在生产者与消费者服务之间引入专门的中间层（broker），负责接收事件并高可靠、高持久性地投递给下游服务，避免直接同步调用带来的脆弱性。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-messaging-queues]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 像 YouTube、Google Drive 这类平台通过在服务间加入具备高持久性（durability）和可靠投递能力的 broker 来解决直接同步调用可能导致事件丢失的问题，这也是不采用服务间直接同步通信的核心原因。（[33:08](https://youtu.be/Qa-7iWxDz1A?t=1988)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[event-fan-out-multiple-subscribers]]
- [[synchronous-downstream-call-risk]]
%% ytkb:end %%
