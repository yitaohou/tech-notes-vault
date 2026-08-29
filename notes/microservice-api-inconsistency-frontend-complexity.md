---
title: Microservice API Inconsistency Frontend Complexity
aliases: []
tags:
- concept
summary: 客户端需要直接调用多个微服务、且各微服务 API 形态各异，导致前端需要为每个 API 维护不同的 client/SDK，增加前端复杂度。
created: '2026-08-26'
updated: '2026-08-26'
---

# Microservice API Inconsistency Frontend Complexity

%% ytkb:def %%
客户端需要直接调用多个微服务、且各微服务 API 形态各异，导致前端需要为每个 API 维护不同的 client/SDK，增加前端复杂度。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-microservices-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 在没有 BFF 的情况下，客户端要对多个形态各异的微服务分别发起 fetch 调用，各自需要不同的 client/SDK，造成大量前端复杂度。（[09:03](https://youtu.be/KuClyhvSzXk?t=543)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[backend-for-frontend-pattern]]
- [[microservices]]
%% ytkb:end %%
