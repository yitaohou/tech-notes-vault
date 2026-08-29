---
title: Map vs Object Iteration
aliases: []
tags:
- concept
summary: Map 与 Object 在遍历方式上的差异，Map 原生支持迭代器，Object 需要借助辅助方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Map vs Object Iteration

%% ytkb:def %%
Map 与 Object 在遍历方式上的差异，Map 原生支持迭代器，Object 需要借助辅助方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 遍历 Object 需要借助 Object.entries() 或 Object.keys()，而 Map 直接内置了 iterator，可以直接被遍历。（[39:09](https://youtu.be/AMerB8XjfZ0?t=2349)）
%% ytkb:end %%
