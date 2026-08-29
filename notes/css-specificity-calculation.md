---
title: CSS Specificity Calculation
aliases: []
tags:
- concept
summary: CSS specificity 是通过分别统计选择器中 ID、class/attribute、element 类型的数量得到的三元组分值，用于决定哪条规则生效。
created: '2026-08-26'
updated: '2026-08-26'
---

# CSS Specificity Calculation

%% ytkb:def %%
CSS specificity 是通过分别统计选择器中 ID、class/attribute、element 类型的数量得到的三元组分值，用于决定哪条规则生效。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-css-styling]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 计算 specificity 时，引用 element 类型（如 form）记一分，class 或 attribute 选择器记一分，ID 选择器单独记一分，三者分属不同位次而非同一累加值。（[27:07](https://youtu.be/AMerB8XjfZ0?t=1627)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[css-specificity-tiebreak-rule]]
%% ytkb:end %%
