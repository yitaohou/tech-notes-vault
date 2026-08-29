---
title: Browser Reflow
aliases: []
tags:
- concept
summary: 浏览器中修改会影响布局的 CSS 属性（如 width）时，触发的重新计算布局的过程，会波及该区域内其他元素并引发完整渲染流程。
created: '2026-08-26'
updated: '2026-08-26'
---

# Browser Reflow

%% ytkb:def %%
浏览器中修改会影响布局的 CSS 属性（如 width）时，触发的重新计算布局的过程，会波及该区域内其他元素并引发完整渲染流程。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-css-styling]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 用 JavaScript 直接修改 button 的 width 属性会触发 reflow，浏览器需要重新扫描该区域所有元素、重新计算宽高等布局属性，进而触发从布局到 GPU 生成像素的完整渲染流程。（[00:00](https://youtu.be/AMerB8XjfZ0?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[css-transform-compositor-thread]]
- [[main-thread-vs-compositor-thread]]
%% ytkb:end %%
