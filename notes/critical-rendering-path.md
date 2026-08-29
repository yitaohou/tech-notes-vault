---
title: Critical Rendering Path
aliases: []
tags:
- concept
summary: 浏览器渲染页面前需要解析、解释大体积 CSS 和 JavaScript 资源的关键路径，是决定页面首次渲染速度的核心环节。
created: '2026-08-26'
updated: '2026-08-26'
---

# Critical Rendering Path

%% ytkb:def %%
浏览器渲染页面前需要解析、解释大体积 CSS 和 JavaScript 资源的关键路径，是决定页面首次渲染速度的核心环节。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 页面加载慢的根本原因通常是发送了过多 JavaScript：critical rendering path 中的大体积 CSS 和 JS 文件需要先被解析、解释后才能进行实际渲染。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- critical rendering path 的具体步骤依次为：构建 DOM、构建 CSSOM、生成 render tree、计算 layout tree（各节点的位置与宽度）、转换为交给 GPU 处理的 paint 操作，最后进入 composite 阶段；组件框架引起的重新渲染会在这些步骤完成后反复触发。（[29:07](https://youtu.be/KuClyhvSzXk?t=1747)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[largest-contentful-paint]]
- [[main-thread-vs-compositor-thread]]
- [[react-bundle-size-analysis]]
- [[react-server-components]]
%% ytkb:end %%
