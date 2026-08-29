---
title: Architectural Drift
aliases: []
tags:
- concept
summary: 指系统的实际实现随着时间推移逐渐偏离其原本设计架构的现象。
created: '2026-08-26'
updated: '2026-08-26'
---

# Architectural Drift

%% ytkb:def %%
指系统的实际实现随着时间推移逐渐偏离其原本设计架构的现象。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-architecture-fundamentals]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- AI 时代优秀的前端系统设计应当最小化架构漂移，让代码演进始终贴合既定架构，从而降低后续人工验证代码的成本。（[00:00](https://youtu.be/KuClyhvSzXk?t=0)）
- 团队若各自使用不同的 TypeScript 配置或 linter 规则，容易导致多个项目产生 architectural drift（code style drift），即项目间代码风格、依赖和质量标准逐渐分化。（[24:07](https://youtu.be/KuClyhvSzXk?t=1447)）
- architectural drift 的负面影响是，开发者换到另一个团队后必须重新学习一套完全不同的代码规范，无法复用已积累的经验，即无法真正实现标准化。（[24:07](https://youtu.be/KuClyhvSzXk?t=1447)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-verification-time-tradeoff]]
- [[monorepo]]
%% ytkb:end %%
