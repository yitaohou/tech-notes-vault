---
title: Object Storage Upload Event Trigger
aliases: []
tags:
- concept
summary: 对象存储在文件上传完成后，向内部系统发送事件通知，触发后续处理动作。
created: '2026-08-26'
updated: '2026-08-26'
---

# Object Storage Upload Event Trigger

%% ytkb:def %%
对象存储在文件上传完成后，向内部系统发送事件通知，触发后续处理动作。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-file-storage]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 文件上传到 bucket 后，对象存储会向内部系统发送一个事件（如「文件已上传」），用于触发诸如实时更新前端、发送推送通知等后续动作。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[message-broker-pub-sub]]
- [[object-storage-bypass-api-server]]
%% ytkb:end %%
