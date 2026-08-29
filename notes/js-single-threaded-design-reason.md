---
title: Why JavaScript Is Single-Threaded
aliases: []
tags:
- concept
summary: JavaScript 被设计为单线程运行的原因说明。
created: '2026-08-26'
updated: '2026-08-26'
---

# Why JavaScript Is Single-Threaded

%% ytkb:def %%
JavaScript 被设计为单线程运行的原因说明。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-javascript-runtime]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- JavaScript 被设计为单线程，主要是为了让 DOM 的渲染结果更容易预测；虽然浏览器本身大多是多线程的，但如果让 JS 也变成多线程执行，会因并行化带来难以预料且危险的 bug，尤其是因为每次修改 JavaScript 都会影响 DOM 这个唯一的单例结构。（[30:08](https://youtu.be/AMerB8XjfZ0?t=1808)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[event-loop-mechanism]]
- [[js-call-stack]]
%% ytkb:end %%
