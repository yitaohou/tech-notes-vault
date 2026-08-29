---
title: CSS Transform via Compositor Thread
aliases: []
tags:
- concept
summary: CSS transform（如 scale）等变换可以跳过布局重算，直接交给专门的 compositor thread 处理，通常可在 GPU 上完成，是比修改布局属性更高效的动画实现方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# CSS Transform via Compositor Thread

%% ytkb:def %%
CSS transform（如 scale）等变换可以跳过布局重算，直接交给专门的 compositor thread 处理，通常可在 GPU 上完成，是比修改布局属性更高效的动画实现方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 用 CSS transition 配合 scale 这类 CSS transform 实现按钮悬停变大效果，可以绕开 reflow，直接交给 compositor thread 处理，因为这是纯数学变换、不需要修改布局树。（[00:00](https://youtu.be/AMerB8XjfZ0?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[browser-reflow]]
- [[main-thread-vs-compositor-thread]]
%% ytkb:end %%
