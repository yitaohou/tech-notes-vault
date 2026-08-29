---
title: Micro-Frontend Shell
aliases: []
tags:
- concept
summary: micro-frontend shell 是负责承载并整合各个独立 micro-frontend 应用的容器应用，统一处理跨应用共享的全局功能。
created: '2026-08-26'
updated: '2026-08-26'
---

# Micro-Frontend Shell

%% ytkb:def %%
micro-frontend shell 是负责承载并整合各个独立 micro-frontend 应用的容器应用，统一处理跨应用共享的全局功能。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-architecture]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- micro-frontend shell 负责处理 auth、routing、language 和 global state（如用户是否登录）等全局功能，并将这些全局状态传递给其内部加载的各个 micro-frontend 应用。（[03:01](https://youtu.be/KuClyhvSzXk?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[micro-frontend-independent-deployment]]
- [[micro-frontends]]
%% ytkb:end %%
