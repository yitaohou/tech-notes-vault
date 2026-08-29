---
title: WeakMap Lacks Iterator
aliases: []
tags:
- concept
summary: WeakMap 没有实现迭代器（iterator）接口，因此无法直接遍历其中的键值对。
created: '2026-08-26'
updated: '2026-08-26'
---

# WeakMap Lacks Iterator

%% ytkb:def %%
WeakMap 没有实现迭代器（iterator）接口，因此无法直接遍历其中的键值对。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- WeakMap 不支持 forEach 或直接遍历其所有 key，必须自己单独保存曾经访问过的 key 才能再次取用，因此编程上使用起来比 Map 更繁琐。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[map-vs-object-iteration]]
%% ytkb:end %%
