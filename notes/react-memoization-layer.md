---
title: React Memoization Layer
aliases: []
tags:
- concept
summary: 通过 memo、useCallback、useMemo 等手段减少 React 不必要的重新渲染，从而提升渲染速度的一层优化机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# React Memoization Layer

%% ytkb:def %%
通过 memo、useCallback、useMemo 等手段减少 React 不必要的重新渲染，从而提升渲染速度的一层优化机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-react-performance]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 排查加载慢问题时，除了 bundle size，还要检查项目的 memorization layer，即是否合理使用了 memo、useCallback、useMemo 来加快渲染、避免重新渲染。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[react-compiler]]
- [[react-memo-prevents-rerender]]
- [[use-callback-use-memo-purpose]]
%% ytkb:end %%
