---
title: Main Thread vs Compositor Thread
aliases: []
tags:
- concept
summary: 浏览器渲染架构中，main thread 负责执行 JavaScript、布局计算与绘制，compositor thread 是独立的另一线程，专门负责如滚动、简单变换等轻量合成操作。
created: '2026-08-26'
updated: '2026-08-26'
---

# Main Thread vs Compositor Thread

%% ytkb:def %%
浏览器渲染架构中，main thread 负责执行 JavaScript、布局计算与绘制，compositor thread 是独立的另一线程，专门负责如滚动、简单变换等轻量合成操作。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- compositor thread 被设计用来高效处理滚动这类操作而不占用 main thread，只要避免触发 reflow，main thread 就能保持空闲去处理 JavaScript 或其他任务，实现动画与逻辑执行互不阻塞。（[00:00](https://youtu.be/AMerB8XjfZ0?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[browser-reflow]]
- [[css-transform-compositor-thread]]
%% ytkb:end %%
