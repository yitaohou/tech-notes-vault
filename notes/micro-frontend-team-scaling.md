---
title: Micro-Frontends for Team Scaling
aliases: []
tags:
- concept
summary: 当有大量开发者同时在同一应用上工作时，将前端拆分为多个 micro-frontend，以获得更好的故障隔离和更小的爆炸半径。
created: '2026-08-26'
updated: '2026-08-26'
---

# Micro-Frontends for Team Scaling

%% ytkb:def %%
当有大量开发者同时在同一应用上工作时，将前端拆分为多个 micro-frontend，以获得更好的故障隔离和更小的爆炸半径。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-architecture]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 只有当有大量开发者同时在同一个前端应用上工作时，才有必要考虑引入 micro-frontend 架构，目的是获得更好的故障隔离模式和更小的爆炸半径，而不是单纯为了应对用户量增长。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 即使后端已拆分为微服务、团队变小变快，若前端仍是 monolith，会因太多人向同一客户端推送代码而容易出错，甚至有人改动全局 CSS 规则影响所有人，最终导致前端团队因沟通协调开销过大而无法继续扩展。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
- micro-frontends 与 microservices 能降低生产环境 bug 的 blast radius，并因 PR 更小、更局部而降低代码变更带来的认知负荷。（[06:02](https://youtu.be/KuClyhvSzXk?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[micro-frontends]]
- [[microservices]]
- [[microservices-suited-for-large-organizations]]
%% ytkb:end %%
