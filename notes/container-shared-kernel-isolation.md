---
title: Container Shared-Kernel Isolation
aliases: []
tags:
- concept
summary: 容器（container）因共享操作系统内核而隔离性弱于虚拟机，但仍能为运行在其中的单个进程提供一定程度的隔离。
created: '2026-08-26'
updated: '2026-08-26'
---

# Container Shared-Kernel Isolation

%% ytkb:def %%
容器（container）因共享操作系统内核而隔离性弱于虚拟机，但仍能为运行在其中的单个进程提供一定程度的隔离。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-containerization]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 容器方案的隔离并非严格意义上的完全隔离，而是因为共享内核（shared kernel），只能为单个进程提供相对较好的隔离性。（[30:08](https://youtu.be/QBHTbtWSECg?t=1808)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[container-per-language-runtime]]
%% ytkb:end %%
