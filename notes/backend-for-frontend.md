---
title: Backend For Frontend (BFF)
aliases: []
tags:
- concept
summary: BFF 是为特定客户端（如 desktop、mobile）量身定制的专属后端层，通过 gateway 路由，使各客户端团队能独立工作且与共享的后端服务解耦。
created: '2026-08-26'
updated: '2026-08-26'
---

# Backend For Frontend (BFF)

%% ytkb:def %%
BFF 是为特定客户端（如 desktop、mobile）量身定制的专属后端层，通过 gateway 路由，使各客户端团队能独立工作且与共享的后端服务解耦。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-microservices-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- BFF 模式下每个客户端都有自己专属的 backend for frontend，客户端团队可以独立开发，同时与真正的后端服务完全解耦。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
- desktop 和 mobile 各自拥有不同的 BFF，它们底层调用相同的后端服务，但对外暴露的 API 结构不同，因为 desktop 通常一次性拉取大量信息，而 mobile 由于屏幕更小需要不同粒度的数据。（[12:04](https://youtu.be/KuClyhvSzXk?t=724)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-gateway]]
- [[graphql]]
- [[over-fetching-under-fetching]]
%% ytkb:end %%
