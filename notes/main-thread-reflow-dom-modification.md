---
title: Main Thread Reflow from DOM Modification
aliases: []
tags:
- concept
summary: 修改 DOM 会触发主线程的 reflow，需要经过 event loop 和调用栈才能完成解释执行的开销机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# Main Thread Reflow from DOM Modification

%% ytkb:def %%
修改 DOM 会触发主线程的 reflow，需要经过 event loop 和调用栈才能完成解释执行的开销机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 修改 DOM 会触发主线程 reflow，这个改动要先压入调用栈、被解释执行，因此应尽量避免频繁触发。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[compositor-thread-layer-promotion]]
%% ytkb:end %%
