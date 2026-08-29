---
title: Microservice Single Responsibility
aliases: []
tags:
- concept
summary: 微服务架构中每个服务只专注承担单一职责的设计原则，是 separation of concerns 在更大规模系统上的体现。
created: '2026-08-26'
updated: '2026-08-26'
---

# Microservice Single Responsibility

%% ytkb:def %%
微服务架构中每个服务只专注承担单一职责的设计原则，是 separation of concerns 在更大规模系统上的体现。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-microservices-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 在微服务架构中，thumbnail service 只负责实时生成缩略图，notification service 只负责实时文件通知，authentication service 只负责认证，各服务职责单一，这本质上是更大规模下的 separation of concerns。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[distributed-architecture-avoid-spof]]
%% ytkb:end %%
