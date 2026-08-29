---
title: Microservices Architecture
aliases: []
tags:
- concept
summary: 将系统拆分成多个各自专精、只负责单一职责的独立服务的架构方式，与单体架构相对。
created: '2026-08-26'
updated: '2026-08-26'
---

# Microservices Architecture

%% ytkb:def %%
将系统拆分成多个各自专精、只负责单一职责的独立服务的架构方式，与单体架构相对。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-microservices-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 当所有请求都由同一批服务器处理时，某一功能（如文件上传）的负载激增会拖慢整个系统，这正是促使系统从单体架构转向 microservices 的常见诱因。（[18:05](https://youtu.be/Qa-7iWxDz1A?t=1085)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 微服务拆分通常从 back-end 开始，把 monolith 拆分成各自暴露独立 API、可独立部署的 micro back-end，代码库和团队彼此独立，只通过 API 相互通信。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[conways-law]]
- [[domain-driven-service-decomposition]]
- [[microservice-blueprint-layers]]
- [[microservices-suited-for-large-organizations]]
- [[single-point-of-failure]]
%% ytkb:end %%
