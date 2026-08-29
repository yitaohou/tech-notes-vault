---
title: Extracting Non-State Logic Out of Components
aliases: []
tags:
- concept
summary: 把不直接依赖组件 state 的逻辑抽离成独立函数放在组件外部，避免该逻辑随组件每次重新渲染而被重复创建的优化手法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Extracting Non-State Logic Out of Components

%% ytkb:def %%
把不直接依赖组件 state 的逻辑抽离成独立函数放在组件外部，避免该逻辑随组件每次重新渲染而被重复创建的优化手法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-react-component-design]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 让组件保持精简的做法是把不直接需要 state 的逻辑抽离成组件外部的独立函数，这样这部分逻辑只在应用加载时创建一次，不会随组件重新渲染而重复创建。（[36:08](https://youtu.be/AMerB8XjfZ0?t=2168)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[use-callback-use-memo-purpose]]
%% ytkb:end %%
