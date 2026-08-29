---
title: Micro-Frontend Independent Deployment
aliases: []
tags:
- concept
summary: 指每个 micro-frontend 应用可以被独立构建、独立部署，甚至托管在各自独立的域名下。
created: '2026-08-26'
updated: '2026-08-26'
---

# Micro-Frontend Independent Deployment

%% ytkb:def %%
指每个 micro-frontend 应用可以被独立构建、独立部署，甚至托管在各自独立的域名下。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-architecture]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 各个 micro-frontend 可以独立部署，例如 header 应用可以托管在 header.theseniordev.com 这样单独的域名下并独立加载，product 页和 cart 页同理，最终由 shell 把它们整合在一起。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[micro-frontend-shell]]
- [[micro-frontends]]
%% ytkb:end %%
