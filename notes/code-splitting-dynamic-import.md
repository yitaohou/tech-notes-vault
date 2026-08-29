---
title: Code Splitting via Dynamic Import
aliases: []
tags:
- concept
summary: 通过动态导入（dynamic import）延迟加载非首屏必需的代码，可按路径或用户操作进行拆分的优化技术。
created: '2026-08-26'
updated: '2026-08-26'
---

# Code Splitting via Dynamic Import

%% ytkb:def %%
通过动态导入（dynamic import）延迟加载非首屏必需的代码，可按路径或用户操作进行拆分的优化技术。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-architecture]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 为了减少首屏加载的 JavaScript 量，应该使用 dynamic import 来延迟加载非必需代码，并可以按路径（path）或用户操作（user actions）进行 code splitting。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 传统 module bundler 会把所有 JavaScript 打包进单个大文件，一次性加载这种大文件会严重拖慢 Core Web Vitals，因为加载了远超当前页面所需的代码量。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
- code splitting 最简单的实现方式是按路由拆分：例如只给 /login 页面发送登录相关组件代码，而像 dashboard 中大量图表这类重量级代码则不随之一起打包发送。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
- Webpack、Vite 等 module bundler 能理解应用的 bundle 结构并对其进行拆分，再配合应用路由器（router），根据用户当前所在路径动态加载对应的代码块。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[lazy-loading-vs-eager-loading]]
- [[react-bundle-size-analysis]]
%% ytkb:end %%
