---
title: Largest Contentful Paint (LCP)
aliases: []
tags:
- concept
summary: 衡量页面加载速度的 Core Web Vitals 指标，指从用户发出请求到页面中最大元素被渲染完成所经过的时间。
created: '2026-08-26'
updated: '2026-08-26'
---

# Largest Contentful Paint (LCP)

%% ytkb:def %%
衡量页面加载速度的 Core Web Vitals 指标，指从用户发出请求到页面中最大元素被渲染完成所经过的时间。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- LCP 指从用户按下回车到页面中最大元素渲染完成所花费的时间，与页面初次渲染相关。（[28:18](https://youtu.be/KuClyhvSzXk?t=1698)）
- 若应用打包体积过大（JS、CSS 过多）、需要拉取大量数据、或服务器响应慢，都会导致 LCP 分数变差。（[29:41](https://youtu.be/KuClyhvSzXk?t=1781)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[code-splitting-dynamic-import]]
- [[core-web-vitals]]
- [[critical-rendering-path]]
- [[react-bundle-size-analysis]]
%% ytkb:end %%
