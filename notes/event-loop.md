---
title: Event Loop
aliases: []
tags:
- concept
summary: JavaScript event loop 是把渲染任务和 JS 执行任务（microtask）交替推送给 CPU 处理的调度机制，用以避免长时间阻塞浏览器
  UI。
created: '2026-08-26'
updated: '2026-08-26'
---

# Event Loop

%% ytkb:def %%
JavaScript event loop 是把渲染任务和 JS 执行任务（microtask）交替推送给 CPU 处理的调度机制，用以避免长时间阻塞浏览器 UI。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- event loop 可以类比为两条并行传送带，把 JS 执行（microtask）和渲染工作交替推送给同一个 CPU：先处理一段 JS，再检查是否有渲染任务要做，处理完再回来处理下一段 JS，如此循环。（[33:08](https://youtu.be/AMerB8XjfZ0?t=1988)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[main-thread-blocking]]
%% ytkb:end %%
