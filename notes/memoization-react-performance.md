---
title: Memoization for Render Performance
aliases: []
tags:
- concept
summary: 通过 memoization 减少不必要的重复计算与重渲染，从而降低推送到主线程栈的工作负担。
created: '2026-08-26'
updated: '2026-08-26'
---

# Memoization for Render Performance

%% ytkb:def %%
通过 memoization 减少不必要的重复计算与重渲染，从而降低推送到主线程栈的工作负担。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-react-performance]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 主线程的任务栈被设计为擅长处理大量微小的独立工作单元，因此应尽量使用 memoization、把每次更新拆成小颗粒度的工作，而不要一次性推送大块任务，尤其在大型组件框架中。（[33:08](https://youtu.be/AMerB8XjfZ0?t=1988)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[event-handler-overload-performance-bug]]
%% ytkb:end %%
