---
title: Component Library Accessibility
aliases: []
tags:
- concept
summary: 指像 dropdown 这类组件若要自行从零实现并做到无障碍（accessible），需要投入大量工作，因此复用现成 accessible 组件库可避免重复造轮子。
created: '2026-08-26'
updated: '2026-08-26'
---

# Component Library Accessibility

%% ytkb:def %%
指像 dropdown 这类组件若要自行从零实现并做到无障碍（accessible），需要投入大量工作，因此复用现成 accessible 组件库可避免重复造轮子。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-accessibility]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 自己实现并做到 accessible 的组件（如 dropdown）成本很高，直接复用现成的 accessible 组件库能避免重复造轮子。（[18:04](https://youtu.be/AMerB8XjfZ0?t=1084)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 设计系统组件库可以统一处理组件的 accessibility，避免每个团队各自重复投入精力实现无障碍能力。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
%% ytkb:end %%

%% ytkb:video:hA_XnzB1Ef8 %%
### 来自 [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof]]
- 如果公司级设计系统（design system）已经把组件的无障碍性（accessibility）做好，AI 在生成组件时可以直接复用该设计系统的能力，工程师只需做一次轻量复核（soft check），而不必从零验证 accessibility。（[12:03](https://youtu.be/hA_XnzB1Ef8?t=723)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[design-system]]
- [[design-token]]
%% ytkb:end %%
