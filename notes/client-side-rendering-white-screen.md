---
title: Client-Side Rendering White Screen Problem
aliases: []
tags:
- concept
summary: 指使用 React、Vue、Angular 等现代组件框架的 SPA 在用户刚打开页面时会先看到白屏，因为初始加载的 HTML 是空的，需等框架渲染函数执行完毕才会显示内容，这种渲染模式称为
  client-side rendering（CSR）。
created: '2026-08-26'
updated: '2026-08-26'
---

# Client-Side Rendering White Screen Problem

%% ytkb:def %%
指使用 React、Vue、Angular 等现代组件框架的 SPA 在用户刚打开页面时会先看到白屏，因为初始加载的 HTML 是空的，需等框架渲染函数执行完毕才会显示内容，这种渲染模式称为 client-side rendering（CSR）。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-rendering-strategies]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 在 client-side rendering 下，浏览器加载的初始 HTML 是空的，只有当框架的渲染函数真正执行后页面才会显示内容，这导致用户短暂看到白屏。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[csr-loading-waterfall]]
%% ytkb:end %%
