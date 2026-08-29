---
title: Compositor Thread Layer Promotion
aliases: []
tags:
- concept
summary: 把元素提升到独立的合成层（layer），使浏览器能用 compositor thread 处理简单变换（如放大），从而绕开主线程的技术手段。
created: '2026-08-26'
updated: '2026-08-26'
---

# Compositor Thread Layer Promotion

%% ytkb:def %%
把元素提升到独立的合成层（layer），使浏览器能用 compositor thread 处理简单变换（如放大），从而绕开主线程的技术手段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 把按钮提升到独立 layer 后，浏览器可以交给 compositor thread 处理像放大这样简单的变换，而不必经过主线程。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[main-thread-reflow-dom-modification]]
%% ytkb:end %%
