---
title: Self-Harness 可编辑范围限制
aliases: []
tags:
- concept
summary: Self-Harness 中对可编辑范围的严格限制，用于防止改进程序直接编辑操作系统而打破系统抽象边界的安全设计原则。
created: '2026-08-26'
updated: '2026-08-26'
---

# Self-Harness 可编辑范围限制

%% ytkb:def %%
Self-Harness 中对可编辑范围的严格限制，用于防止改进程序直接编辑操作系统而打破系统抽象边界的安全设计原则。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- 如果允许 Self-Harness 的改进程序编辑操作系统，系统的抽象边界就会被打破，因此可编辑范围必须严格设计，权限控制和安全层必须置于自改进循环之外。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[self-harness]]
%% ytkb:end %%
