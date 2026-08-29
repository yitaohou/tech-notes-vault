---
title: CSR Loading Waterfall
aliases: []
tags:
- concept
summary: 指采用 client-side rendering 的单页应用中，页面加载须依次经过获取静态文件、获取动态数据、最终渲染三个阶段，整体耗时较长的加载链路。
created: '2026-08-26'
updated: '2026-08-26'
---

# CSR Loading Waterfall

%% ytkb:def %%
指采用 client-side rendering 的单页应用中，页面加载须依次经过获取静态文件、获取动态数据、最终渲染三个阶段，整体耗时较长的加载链路。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-rendering-strategies]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 在采用 client-side rendering 的 SPA 架构中，加载顺序依次是获取静态文件、再获取动态数据、最后才执行渲染，这一整套流程会耗费较长时间。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[client-side-rendering-white-screen]]
%% ytkb:end %%
