---
title: Worker Pull Pattern
aliases: []
tags:
- concept
summary: worker 主动从消息队列中拉取任务执行、完成后再更新状态的任务处理模式，与队列主动推送任务相对。
created: '2026-08-26'
updated: '2026-08-26'
---

# Worker Pull Pattern

%% ytkb:def %%
worker 主动从消息队列中拉取任务执行、完成后再更新状态的任务处理模式，与队列主动推送任务相对。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-microservices-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 在基于队列的架构中，runtime server 作为 worker 主动从队列中拉取（pull）待执行的提交任务，执行完成后更新数据库和缓存。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 以订单处理为例：producer 在新订单产生时向队列发布消息，consumer 仅在自己有空闲处理能力时才从队列中拉取消息并更新库存数据；若 consumer 正忙，消息会留在队列中等待其下次有空闲容量时再被拉取处理。（[54:11](https://youtu.be/oYxTTirKY8M?t=3251)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[message-broker-pub-sub]]
- [[message-queue-load-smoothing]]
%% ytkb:end %%
