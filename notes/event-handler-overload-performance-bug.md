---
title: Event Handler Overload Performance Bug
aliases: []
tags:
- concept
summary: 指在组件框架中因绑定过多事件处理器（event handler）、导致主线程任务栈过重而引发的常见前端性能问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# Event Handler Overload Performance Bug

%% ytkb:def %%
指在组件框架中因绑定过多事件处理器（event handler）、导致主线程任务栈过重而引发的常见前端性能问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 最常见的与 event loop 相关的生产环境 bug 是表单里绑定了过多事件处理器，用户打字时触发大量重渲染任务被推入栈中，导致输入出现明显卡顿（lagging）。（[33:08](https://youtu.be/AMerB8XjfZ0?t=1988)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[main-thread-blocking]]
- [[memoization-react-performance]]
%% ytkb:end %%
