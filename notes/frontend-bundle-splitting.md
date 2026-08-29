---
title: Frontend Bundle Splitting
aliases: []
tags:
- concept
summary: 在 Webpack 或 Vite 等构建工具层面，把前端应用拆分成多个 chunk（如稳定依赖与业务逻辑分开）的技术。
created: '2026-08-26'
updated: '2026-08-26'
---

# Frontend Bundle Splitting

%% ytkb:def %%
在 Webpack 或 Vite 等构建工具层面，把前端应用拆分成多个 chunk（如稳定依赖与业务逻辑分开）的技术。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-architecture]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 对纯 client-rendered 前端应用做扩展时，第一步通常是把静态资源（JS、HTML、CSS）推送到 CDN，并在此基础上做 bundle splitting，而不是简单地整体推送单一 bundle。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cdn-edge-asset-caching]]
- [[selective-caching-policy-frontend]]
%% ytkb:end %%
