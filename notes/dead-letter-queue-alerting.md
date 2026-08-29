---
title: Dead Letter Queue Alerting
aliases: []
tags:
- concept
summary: 针对进入 dead letter queue 的消息设置告警通知（如发送到 Slack、Discord），以便及时发现哪条消息未能成功送达。
created: '2026-08-26'
updated: '2026-08-26'
---

# Dead Letter Queue Alerting

%% ytkb:def %%
针对进入 dead letter queue 的消息设置告警通知（如发送到 Slack、Discord），以便及时发现哪条消息未能成功送达。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-messaging-queues]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 需要为 dead letter queue 配置告警机制，将未送达的消息信息发送到 Slack 或 Discord 等渠道，从而及时知晓具体是哪条消息投递失败。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dead-letter-queue]]
%% ytkb:end %%
