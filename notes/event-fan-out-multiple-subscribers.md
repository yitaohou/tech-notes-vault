---
title: Event Fan-out to Multiple Subscribers
aliases: []
tags:
- concept
summary: 同一个事件（如文件上传完成）需要被同时投递给多个下游订阅者（如缩略图服务、实时同步服务）的场景。
created: '2026-08-26'
updated: '2026-08-26'
---

# Event Fan-out to Multiple Subscribers

%% ytkb:def %%
同一个事件（如文件上传完成）需要被同时投递给多个下游订阅者（如缩略图服务、实时同步服务）的场景。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-messaging-queues]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 一个视频上传事件可能需要同时触发缩略图生成服务和跨设备实时同步服务两个完全不同的下游处理逻辑，这种一对多投递需求称为 fan-out。（[33:08](https://youtu.be/Qa-7iWxDz1A?t=1988)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[message-broker-necessity]]
- [[producer-consumer-coupling-scalability]]
%% ytkb:end %%
