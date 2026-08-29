---
title: WeakMap Garbage Collection
aliases: []
tags:
- concept
summary: WeakMap 中若某个 key 所指向的对象不再被外部引用（不可达），垃圾回收器会自动将该键值对从 WeakMap 中移除。
created: '2026-08-26'
updated: '2026-08-26'
---

# WeakMap Garbage Collection

%% ytkb:def %%
WeakMap 中若某个 key 所指向的对象不再被外部引用（不可达），垃圾回收器会自动将该键值对从 WeakMap 中移除。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 与 Map 不同，WeakMap 中一旦某个 key 不再被引用（不可达），垃圾回收算法会自动将其从 WeakMap 中移除，从而避免内存泄漏。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[garbage-collection-reachability]]
- [[map-garbage-collection-limitation]]
%% ytkb:end %%
