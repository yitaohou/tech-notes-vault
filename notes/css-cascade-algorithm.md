---
title: CSS Cascade Algorithm
aliases: []
tags:
- concept
summary: cascade algorithm 是浏览器收集所有指向同一元素的 CSS 规则后，用于计算并决定最终生效样式的复杂算法。
created: '2026-08-26'
updated: '2026-08-26'
---

# CSS Cascade Algorithm

%% ytkb:def %%
cascade algorithm 是浏览器收集所有指向同一元素的 CSS 规则后，用于计算并决定最终生效样式的复杂算法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-css-styling]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 当多条 CSS 规则的 selector 都指向同一个元素时，浏览器会收集这些规则并执行 cascade algorithm 来确定最终样式；若这些规则处于同一 layer，其中一步就是比较各 selector 的 specificity 得分。（[24:07](https://youtu.be/AMerB8XjfZ0?t=1447)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[css-specificity]]
%% ytkb:end %%
