---
title: Interaction to Next Paint (INP)
aliases: []
tags:
- concept
summary: 衡量页面交互速度的 Core Web Vitals 指标，指用户发生交互后到界面完成重新绘制所经过的时间。
created: '2026-08-26'
updated: '2026-08-26'
---

# Interaction to Next Paint (INP)

%% ytkb:def %%
衡量页面交互速度的 Core Web Vitals 指标，指用户发生交互后到界面完成重新绘制所经过的时间。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- INP 衡量的是用户发生交互后到界面完成重新绘制（repaint）所需的时间，与页面初次渲染无关，而是关注后续的重新渲染过程，这对使用组件框架的应用尤为重要。（[28:35](https://youtu.be/KuClyhvSzXk?t=1715)）
- 组件 re-render 过慢或用户操作后重新渲染了过多组件，都会导致 INP（Interaction to Next Paint）指标变差。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[core-web-vitals]]
- [[event-handler-overload-performance-bug]]
- [[main-thread-blocking]]
%% ytkb:end %%
