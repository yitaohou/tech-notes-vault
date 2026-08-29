---
title: Per-Language Runtime Containers
aliases: []
tags:
- concept
summary: 为每种支持的编程语言分别部署独立的 runtime container，使各语言执行环境可以独立扩展和维护的架构设计。
created: '2026-08-26'
updated: '2026-08-26'
---

# Per-Language Runtime Containers

%% ytkb:def %%
为每种支持的编程语言分别部署独立的 runtime container，使各语言执行环境可以独立扩展和维护的架构设计。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 在多语言代码执行系统中，可以为每种编程语言配置专属的 runtime container，并让这些容器各自独立进行水平扩展。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[horizontal-scaling]]
%% ytkb:end %%
