---
title: API Service Boundary
aliases: []
tags:
- concept
summary: API 通过在组件之间定义清晰接口来划定服务边界，使不同系统可以独立实现各自功能并解耦通信。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Service Boundary

%% ytkb:def %%
API 通过在组件之间定义清晰接口来划定服务边界，使不同系统可以独立实现各自功能并解耦通信。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-microservices-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- API 为系统划定了清晰的服务边界，因此可以拆分出多个各自独立负责的服务（如专门管理用户的服务、专门管理帖子的服务），不同服务或客户端与服务端之间可以在互不了解底层实现的前提下正常通信。（[30:03](https://youtu.be/oYxTTirKY8M?t=1803)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-definition]]
- [[microservices]]
%% ytkb:end %%
