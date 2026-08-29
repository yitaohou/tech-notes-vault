---
title: JS Engine vs Browser Runtime Separation
aliases: []
tags:
- concept
summary: JavaScript 引擎（如 V8）与浏览器运行时在事件循环相关组件上的职责划分。
created: '2026-08-26'
updated: '2026-08-26'
---

# JS Engine vs Browser Runtime Separation

%% ytkb:def %%
JavaScript 引擎（如 V8）与浏览器运行时在事件循环相关组件上的职责划分。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 调用栈、microtask 队列和 macrotask 队列这些结构都存在于 V8 引擎内部，而事件循环（event loop）本身并不属于 V8 引擎，而是由浏览器用 C++ 实现的。（[30:08](https://youtu.be/AMerB8XjfZ0?t=1808)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[event-loop-mechanism]]
- [[js-call-stack]]
- [[js-microtask-macrotask-queue]]
%% ytkb:end %%
