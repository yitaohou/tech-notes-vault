---
title: Garbage Collection Reachability
aliases: []
tags:
- concept
summary: JavaScript 垃圾回收判断对象是否可回收的核心依据：该对象是否仍能从程序顶层（如 DOM、事件处理器）被访问到。
created: '2026-08-26'
updated: '2026-08-26'
---

# Garbage Collection Reachability

%% ytkb:def %%
JavaScript 垃圾回收判断对象是否可回收的核心依据：该对象是否仍能从程序顶层（如 DOM、事件处理器）被访问到。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 垃圾回收算法判断一个对象是否可回收，依据是它是否仍然"可达"（reachable），即是否与 DOM 或事件处理器等保持关联；若不再关联，垃圾回收器会将其标记为可重新分配的内存。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[map-garbage-collection-limitation]]
%% ytkb:end %%
