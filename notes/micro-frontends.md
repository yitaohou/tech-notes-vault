---
title: Micro-Frontends
aliases: []
tags:
- concept
summary: 把前端 monolith 拆分为多个独立部署与维护的前端服务的架构方式，类似前端领域的 microservices。
created: '2026-08-26'
updated: '2026-08-26'
---

# Micro-Frontends

%% ytkb:def %%
把前端 monolith 拆分为多个独立部署与维护的前端服务的架构方式，类似前端领域的 microservices。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-architecture]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 当很多人共同贡献同一个前端代码库时，采用 micro-frontends 架构可以缩小单次改动出错的影响范围（blast radius），便于控制损害。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 解决前端团队规模瓶颈的方法是仿照后端从 monolith 拆分为 microservices 的思路，把前端 monolith 拆分成多个可独立部署的 micro-frontend 应用。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
- micro-frontends 的核心思路是把一个前端应用拆分为多个独立的前端应用，再组合到一起，以解决单体前端团队协作规模过大的问题。（[00:00](https://youtu.be/KuClyhvSzXk?t=0)）
- 把架构拆分为 micro-frontend 和多个 microservice 后，各服务可能采用不同技术栈（如 Python、Node.js、Vue.js、Next.js），这使得统一部署变得复杂，是引入 Docker 等标准化部署技术的直接动机。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
- 多个 micro frontend 各自维护独立的 GitHub 仓库（如 shell、payment、inventory），会导致代码分散在成百上千个仓库中，这是 micro frontend 常见的组织问题之一。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[docker]]
- [[frontend-monolith]]
- [[micro-frontend-shell]]
- [[micro-frontend-team-scaling]]
- [[microservices]]
- [[monorepo]]
%% ytkb:end %%
