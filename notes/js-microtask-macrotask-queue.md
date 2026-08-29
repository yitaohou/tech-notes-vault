---
title: Microtask Queue vs Macrotask Queue
aliases: []
tags:
- concept
summary: JavaScript 运行时中用于管理异步回调执行顺序的两种任务队列。
created: '2026-08-26'
updated: '2026-08-26'
---

# Microtask Queue vs Macrotask Queue

%% ytkb:def %%
JavaScript 运行时中用于管理异步回调执行顺序的两种任务队列。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- JavaScript 运行时除了调用栈外还维护 microtask 队列和 macrotask 队列：Promise resolve 后的回调（如 .then）不会直接压入调用栈，而是先进入 microtask 队列；浏览器事件（如 click）触发的事件处理函数或定时器（timer）回调则会进入 macrotask 队列。（[30:08](https://youtu.be/AMerB8XjfZ0?t=1808)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[event-loop-mechanism]]
- [[js-call-stack]]
%% ytkb:end %%
