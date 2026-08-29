---
title: Feature Envy
aliases: []
tags:
- concept
summary: 一种代码异味（code smell），指某处理特定业务的代码总是跑去读取另一个模块的数据来计算，说明这段逻辑放错了位置。
created: '2026-08-26'
updated: '2026-08-26'
---

# Feature Envy

%% ytkb:def %%
一种代码异味（code smell），指某处理特定业务的代码总是跑去读取另一个模块的数据来计算，说明这段逻辑放错了位置。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-code-quality-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:aR97E7aKEgg %%
### 来自 [[2026-07-22-700-萬人下載的-grill-mematt-pocock-到底寫了什麼]]
- 如果处理订单的代码总是跑去存货相关文件里取数据来算，就说明这段逻辑放错了位置，应该搬去订单自己的文件里，这种代码异味叫做 Feature Envy。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[data-clumps]]
- [[refactoring-book]]
%% ytkb:end %%
