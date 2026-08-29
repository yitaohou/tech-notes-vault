---
title: Hydration
aliases: []
tags:
- concept
summary: 客户端收到服务端预渲染的HTML后，执行JavaScript在内存中构建virtual DOM并将其关联到已有DOM节点、使页面从静态变为可交互的过程。
created: '2026-08-26'
updated: '2026-08-26'
---

# Hydration

%% ytkb:def %%
客户端收到服务端预渲染的HTML后，执行JavaScript在内存中构建virtual DOM并将其关联到已有DOM节点、使页面从静态变为可交互的过程。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-rendering-strategies]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- SSR 返回的 HTML 页面虽然避免了白屏，但此时页面还不可交互，因为浏览器尚未构建 virtual DOM 并将其附加到已渲染好的 DOM 上，这一过程称为 hydration。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
- 完成 hydration 之后，应用可能仍需要发起额外的数据请求，即再次访问后端获取更多数据。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[server-side-rendering]]
%% ytkb:end %%
