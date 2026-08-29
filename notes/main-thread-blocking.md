---
title: Main Thread Blocking
aliases: []
tags:
- concept
summary: 指 JS 执行与浏览器渲染共享同一个主线程空间，因而同一时刻只能二选一执行，这也是 JavaScript 被称为阻塞式的原因。
created: '2026-08-26'
updated: '2026-08-26'
---

# Main Thread Blocking

%% ytkb:def %%
指 JS 执行与浏览器渲染共享同一个主线程空间，因而同一时刻只能二选一执行，这也是 JavaScript 被称为阻塞式的原因。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- JS 执行和 DOM 渲染共享同一个主线程（CPU）处理空间，任意时刻只能执行其中一项，这是浏览器有意为之的设计，而不是拆分成两个可并行的独立线程。（[33:08](https://youtu.be/AMerB8XjfZ0?t=1988)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dom-modification-during-render-risk]]
- [[event-loop]]
%% ytkb:end %%
