---
title: Cumulative Layout Shift (CLS)
aliases: []
tags:
- concept
summary: 衡量视觉稳定性的 Core Web Vitals 指标，指页面加载过程中可见元素发生位置偏移的累积程度。
created: '2026-08-26'
updated: '2026-08-26'
---

# Cumulative Layout Shift (CLS)

%% ytkb:def %%
衡量视觉稳定性的 Core Web Vitals 指标，指页面加载过程中可见元素发生位置偏移的累积程度。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- CLS 衡量页面加载过程中 UI 发生位移变化的程度，浏览器会截取页面前后的快照来判断元素是否移动过多。（[28:29](https://youtu.be/KuClyhvSzXk?t=1709)）
- 应用优化不足时，CSS、字体、数据等资源分批延迟到达会导致页面持续发生布局位移，这正是造成 CLS 分数变差的原因。（[29:56](https://youtu.be/KuClyhvSzXk?t=1796)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[core-web-vitals]]
%% ytkb:end %%
