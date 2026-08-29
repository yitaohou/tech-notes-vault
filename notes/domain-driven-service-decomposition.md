---
title: Domain-Driven Service Decomposition
aliases: []
tags:
- concept
summary: 按业务领域边界将系统拆分为多个独立服务的设计方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Domain-Driven Service Decomposition

%% ytkb:def %%
按业务领域边界将系统拆分为多个独立服务的设计方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-microservices-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 一个 Google Drive clone 可按业务领域拆分为四个独立微服务：file service（处理文件上传下载）、notification service（处理 push、web、desktop 通知）、auth service（处理认证）、real-time service（处理多台个人设备之间的实时同步，如本地上传后同步到云端再同步到其他设备）。（[18:05](https://youtu.be/Qa-7iWxDz1A?t=1085)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[microservices-architecture]]
%% ytkb:end %%
