---
title: React.memo Prevents Unnecessary Re-renders
aliases: []
tags:
- concept
summary: React.memo 通过比较组件接收到的 props 是否变化，来避免因父组件重新渲染而引发的子组件不必要重新渲染。
created: '2026-08-26'
updated: '2026-08-26'
---

# React.memo Prevents Unnecessary Re-renders

%% ytkb:def %%
React.memo 通过比较组件接收到的 props 是否变化，来避免因父组件重新渲染而引发的子组件不必要重新渲染。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-react-performance]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- React.memo 会比较组件的 props，如果收到的 props 没有变化，就不会仅因为父组件重新渲染而重新渲染该子组件。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rerender-optimization-strategies]]
%% ytkb:end %%
