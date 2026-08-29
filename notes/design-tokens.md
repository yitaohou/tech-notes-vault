---
title: Design Tokens
aliases: []
tags:
- concept
summary: 用 CSS custom properties 等方式在根元素统一定义品牌色、间距等可复用设计值，作为设计系统的基础层。
created: '2026-08-26'
updated: '2026-08-26'
---

# Design Tokens

%% ytkb:def %%
用 CSS custom properties 等方式在根元素统一定义品牌色、间距等可复用设计值，作为设计系统的基础层。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-design-systems]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 设计系统的第一步是定义 design tokens，通常以 CSS custom properties 形式存储在根元素上（如品牌色变量），供所有组件复用，使全局样式变更（如换品牌色）只需一行代码即可完成。（[15:02](https://youtu.be/AMerB8XjfZ0?t=902)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 构建设计系统的第一步是定义design tokens，即团队的品牌色、border定义、字体家族等视觉基础信息；现代做法是把这些值定义为CSS custom properties。（[20:35](https://youtu.be/KuClyhvSzXk?t=1235)）
- 结合 design tokens 与 Atomic CSS 方法论，可以先定义好某个属性（如 border），再创建对应的原子类（如 .border），其他开发者只需直接使用该类即可，无需重复定义样式。（[21:07](https://youtu.be/KuClyhvSzXk?t=1267)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[atomic-css]]
- [[design-system]]
%% ytkb:end %%
