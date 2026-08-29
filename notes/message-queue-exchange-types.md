---
title: Message Queue Exchange Types
aliases: []
tags:
- concept
summary: 消息队列中 exchange 决定消息如何被路由到队列，常见类型包括一对一的 direct exchange、广播式的 fan-out exchange
  以及基于主题匹配的 topic-based exchange。
created: '2026-08-26'
updated: '2026-08-26'
---

# Message Queue Exchange Types

%% ytkb:def %%
消息队列中 exchange 决定消息如何被路由到队列，常见类型包括一对一的 direct exchange、广播式的 fan-out exchange 以及基于主题匹配的 topic-based exchange。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-messaging-queues]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 消息队列的 exchange 类型主要分为 direct（一对一）、fan-out（广播）和 topic-based（基于主题）三种。（[54:11](https://youtu.be/oYxTTirKY8M?t=3251)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[message-broker-pub-sub]]
%% ytkb:end %%
