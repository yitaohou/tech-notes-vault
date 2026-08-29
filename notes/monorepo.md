---
title: Monorepo
aliases: []
tags:
- concept
summary: 把多个原本独立的应用放进同一个代码仓库、并配合统一 tooling 管理的架构方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Monorepo

%% ytkb:def %%
把多个原本独立的应用放进同一个代码仓库、并配合统一 tooling 管理的架构方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-microservices-architecture]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- monorepo 通过让所有子项目共享同一套代码规范、依赖和构建工具链，能够有效避免 architectural drift。（[24:07](https://youtu.be/KuClyhvSzXk?t=1447)）
- 在 monorepo 中，运行一次如 `npm run build` 的命令，仓库内的各个应用会分别独立完成各自的构建。（[24:07](https://youtu.be/KuClyhvSzXk?t=1447)）
- 为解决 micro frontend 架构下代码分散在大量独立仓库、彼此容易出现不一致的问题，前端系统设计的下一个核心概念就是引入 monorepo。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[architectural-drift]]
- [[micro-frontends]]
%% ytkb:end %%
