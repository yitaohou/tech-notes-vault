---
title: Server-Side Rendering (SSR)
aliases: []
tags:
- concept
summary: 一种渲染策略：客户端请求前端服务器，前端服务器再向后端服务器请求数据并在服务端完成渲染，最终把预渲染好的完整HTML返回给客户端。
created: '2026-08-26'
updated: '2026-08-26'
---

# Server-Side Rendering (SSR)

%% ytkb:def %%
一种渲染策略：客户端请求前端服务器，前端服务器再向后端服务器请求数据并在服务端完成渲染，最终把预渲染好的完整HTML返回给客户端。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-rendering-strategies]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 在 server-side rendering 中，front-end server 会先向 back-end server 请求数据、在服务端完成渲染，再把预渲染好的完整 HTML 页面返回给客户端，因此客户端不会遇到白屏问题。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
- SSR 是前端架构中最复杂的方案之一，只应在确实需要极致性能或 SEO 的场景下使用；很多团队盲目采用 SSR 属于过度工程化，就像开着 F1 赛车去买菜，反而会引入更多问题并让系统整体变慢。（[33:07](https://youtu.be/KuClyhvSzXk?t=1987)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[edge-computing-ssr]]
- [[hydration]]
%% ytkb:end %%
