---
title: Lazy Loading vs Eager Loading
aliases: []
tags:
- concept
summary: eager loading 指用户一到达页面就把所有内容全部加载完毕，lazy loading 则是仅在真正需要时（如滚动到某处、访问某页面、点击某元素）才加载对应内容，是
  code splitting 背后更高层次的心智模型。
created: '2026-08-26'
updated: '2026-08-26'
---

# Lazy Loading vs Eager Loading

%% ytkb:def %%
eager loading 指用户一到达页面就把所有内容全部加载完毕，lazy loading 则是仅在真正需要时（如滚动到某处、访问某页面、点击某元素）才加载对应内容，是 code splitting 背后更高层次的心智模型。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- lazy loading 与 eager loading 相对：前者按需（滚动、跳转、点击等用户交互）逐步加载内容，后者在用户落地页面时就一次性加载全部内容。（[30:07](https://youtu.be/KuClyhvSzXk?t=1807)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[code-splitting-dynamic-import]]
%% ytkb:end %%
