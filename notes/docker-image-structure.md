---
title: Docker Image Structure
aliases: []
tags:
- concept
summary: Docker image 是打包完成的产物，包含应用代码、对应运行时和操作系统三层内容。
created: '2026-08-26'
updated: '2026-08-26'
---

# Docker Image Structure

%% ytkb:def %%
Docker image 是打包完成的产物，包含应用代码、对应运行时和操作系统三层内容。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-containerization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 以 Next.js 应用为例，其 Docker image 会包含应用代码本身、Next.js 所需的 Node.js runtime，以及底层操作系统（通常是 Linux）。（[15:04](https://youtu.be/KuClyhvSzXk?t=904)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[docker]]
- [[dockerfile]]
%% ytkb:end %%
