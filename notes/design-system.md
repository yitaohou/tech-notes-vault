---
title: Design System
aliases: []
tags:
- concept
summary: 由 design tokens、可复用组件等构成的一套体系，为产品提供统一的视觉规范并加快 AI 辅助开发速度。
created: '2026-08-26'
updated: '2026-08-26'
---

# Design System

%% ytkb:def %%
由 design tokens、可复用组件等构成的一套体系，为产品提供统一的视觉规范并加快 AI 辅助开发速度。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-design-systems]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 构建一个好的设计系统能让 AI 辅助开发更快，并为界面提供视觉一致性（visual cohesion），其第一步是提炼出 design tokens。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 在 feature team / platform team 组织架构中，设计系统（design system）通常由 platform team 构建并维护，供各 feature team 复用。（[00:00](https://youtu.be/KuClyhvSzXk?t=0)）
- 设计系统能够同时解决micro-frontend架构下的代码重复问题和视觉不一致（divergence）问题，是构建统一产品体验的关键手段。（[20:20](https://youtu.be/KuClyhvSzXk?t=1220)）
- 设计系统组件库还可以为其所有组件编写统一的单元测试，保证组件质量并减轻各团队重复测试的负担。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
- 拥有完善的设计系统，是决定 AI coding agent 输出的是杂乱不一致的组件与需要大量返工的 bug，还是稳定可靠代码的关键差异。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
- 启动新 AI 辅助项目时的最佳实践是先从已有设计稿中提取出设计系统，再把它喂给 coding agent，从而在多个会话之间保持生成代码风格的一致性。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[component-library-accessibility]]
- [[design-tokens]]
- [[feature-team-platform-team-split]]
- [[micro-frontend-visual-divergence]]
- [[reusable-components]]
- [[vibe-coding]]
%% ytkb:end %%
