---
title: WeakMap for Function Memoization
aliases: []
tags:
- concept
summary: 利用 WeakMap 的自动垃圾回收特性为函数结果做缓存（memoization），避免手动管理缓存对象的内存释放。
created: '2026-08-26'
updated: '2026-08-26'
---

# WeakMap for Function Memoization

%% ytkb:def %%
利用 WeakMap 的自动垃圾回收特性为函数结果做缓存（memoization），避免手动管理缓存对象的内存释放。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 当需要为函数做 memoization（结果缓存）时，使用 WeakMap 比普通 Map 或 Object 更安全、更省内存，因为不再使用的缓存 key 会被自动垃圾回收。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[weakmap-garbage-collection]]
%% ytkb:end %%
