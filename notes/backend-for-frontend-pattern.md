---
title: Backend for Frontend (BFF)
aliases: []
tags:
- concept
summary: 一种介于客户端与多个微服务之间的专属后端层，由前端团队自己拥有，负责聚合转发请求给各微服务，使前端团队能像 full-stack 一样端到端拥有客户端功能。
created: '2026-08-26'
updated: '2026-08-26'
---

# Backend for Frontend (BFF)

%% ytkb:def %%
一种介于客户端与多个微服务之间的专属后端层，由前端团队自己拥有，负责聚合转发请求给各微服务，使前端团队能像 full-stack 一样端到端拥有客户端功能。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-microservices-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- BFF 接收前端请求后转发给对应微服务，前端团队借此可以整合改造微服务接口，自行实现新功能，端到端拥有客户端侧的整个特性交付。（[09:03](https://youtu.be/KuClyhvSzXk?t=543)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-gateway]]
- [[backend-team-backlog-bottleneck]]
- [[microservice-api-inconsistency-frontend-complexity]]
- [[microservices]]
%% ytkb:end %%
