---
title: Event Loop Execution Mechanism
aliases: []
tags:
- concept
summary: 事件循环协调调用栈与任务队列、决定代码执行顺序的具体工作机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# Event Loop Execution Mechanism

%% ytkb:def %%
事件循环协调调用栈与任务队列、决定代码执行顺序的具体工作机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 事件循环会先检查主线程是否空闲，空闲时执行调用栈中的所有任务；调用栈清空后再检查 microtask 队列，若队列中有任务就将其压入栈底执行；一个 microtask 执行完毕后不会立刻连续处理下一个，而是先检查主线程是否需要进行渲染。（[30:08](https://youtu.be/AMerB8XjfZ0?t=1808)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[js-call-stack]]
- [[js-engine-vs-browser-runtime-split]]
- [[js-microtask-macrotask-queue]]
%% ytkb:end %%
