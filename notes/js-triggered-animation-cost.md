---
title: JavaScript-Triggered Layout Animation Cost
aliases: []
tags:
- concept
summary: 用 JavaScript 反复修改布局属性（如 width）来实现动画效果，会比纯 CSS 方案更昂贵，因为它同时占用 main thread 执行
  JS 逻辑并触发布局重算。
created: '2026-08-26'
updated: '2026-08-26'
---

# JavaScript-Triggered Layout Animation Cost

%% ytkb:def %%
用 JavaScript 反复修改布局属性（如 width）来实现动画效果，会比纯 CSS 方案更昂贵，因为它同时占用 main thread 执行 JS 逻辑并触发布局重算。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 如果动画效果是通过 JavaScript 在 mouseenter 事件里修改 width 实现的，比单纯用 CSS 触发 reflow 更差，因为它还额外占用了 main thread 去执行 JavaScript 逻辑。（[00:00](https://youtu.be/AMerB8XjfZ0?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[browser-reflow]]
- [[main-thread-vs-compositor-thread]]
%% ytkb:end %%
