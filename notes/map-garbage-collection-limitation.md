---
title: Map Cannot Be Garbage Collected
aliases: []
tags:
- concept
summary: JavaScript 的 Map 结构中，即使某个 key 所指向的对象已不再被使用，垃圾回收算法也无法进入 Map 内部对其进行回收。
created: '2026-08-26'
updated: '2026-08-26'
---

# Map Cannot Be Garbage Collected

%% ytkb:def %%
JavaScript 的 Map 结构中，即使某个 key 所指向的对象已不再被使用，垃圾回收算法也无法进入 Map 内部对其进行回收。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- Map 中的 key 即使指向已不再需要的对象，也不会被垃圾回收，如果持续往 Map 添加内容而不手动清理，会导致内存泄漏（memory leak）。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[weakmap-garbage-collection]]
%% ytkb:end %%
