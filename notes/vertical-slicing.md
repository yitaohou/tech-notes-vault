---
title: Vertical Slicing
aliases: []
tags:
- concept
summary: 把 micro-frontend 与 microservices 按业务领域垂直组合、由单一团队独立负责开发和发布的架构切分方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Vertical Slicing

%% ytkb:def %%
把 micro-frontend 与 microservices 按业务领域垂直组合、由单一团队独立负责开发和发布的架构切分方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-microservices-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 当 micro-frontend 与同一业务领域内的一个或多个 microservices 组合在一起时，就形成了 vertical slice，可以由独立团队扩展和维护。（[06:02](https://youtu.be/KuClyhvSzXk?t=362)）
- 采用 vertical slicing 后，团队可以独立发布变更，不会成为其他团队的瓶颈，同时通过 API 与其他团队协作。（[06:02](https://youtu.be/KuClyhvSzXk?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[micro-frontends]]
- [[microservices]]
%% ytkb:end %%
