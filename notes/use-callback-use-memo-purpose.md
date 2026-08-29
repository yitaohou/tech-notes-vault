---
title: useCallback and useMemo Purpose
aliases: []
tags:
- concept
summary: useCallback 和 useMemo 用于确保组件内声明的函数或变量不会在每次重新渲染时被重复计算，从而提升渲染效率。
created: '2026-08-26'
updated: '2026-08-26'
---

# useCallback and useMemo Purpose

%% ytkb:def %%
useCallback 和 useMemo 用于确保组件内声明的函数或变量不会在每次重新渲染时被重复计算，从而提升渲染效率。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-react-performance]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 当组件确实需要重新渲染时，使用 useCallback 和 useMemo 可以确保组件内声明的变量和函数不会被不必要地重新计算。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[react-memoization-layer]]
- [[rerender-optimization-strategies]]
%% ytkb:end %%
