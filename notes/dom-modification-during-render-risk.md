---
title: DOM Modification During Render Risk
aliases: []
tags:
- concept
summary: 指若允许在渲染过程中同时修改 DOM，会破坏 UI 状态一致性、并让编程模型变得过于复杂的风险。
created: '2026-08-26'
updated: '2026-08-26'
---

# DOM Modification During Render Risk

%% ytkb:def %%
指若允许在渲染过程中同时修改 DOM，会破坏 UI 状态一致性、并让编程模型变得过于复杂的风险。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-rendering-strategies]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 浏览器不允许在渲染的同时修改 DOM，因为这会破坏 UI 状态、且让编程模型难以处理，所以刻意把 JS 执行与渲染设计为互斥的两个阶段。（[33:08](https://youtu.be/AMerB8XjfZ0?t=1988)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[main-thread-blocking]]
%% ytkb:end %%
