---
title: JavaScript Call Stack
aliases: []
tags:
- concept
summary: JavaScript 运行时中用于执行函数调用的栈结构。
created: '2026-08-26'
updated: '2026-08-26'
---

# JavaScript Call Stack

%% ytkb:def %%
JavaScript 运行时中用于执行函数调用的栈结构。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 每当执行一个函数时，会将其压入调用栈（call stack）形成一个栈帧（stack frame），栈帧内保存该函数的闭包（closures）和所有会用到的变量，用于实际执行该函数。（[30:08](https://youtu.be/AMerB8XjfZ0?t=1808)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[event-loop-mechanism]]
- [[js-microtask-macrotask-queue]]
%% ytkb:end %%
