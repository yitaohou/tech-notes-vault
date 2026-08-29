---
title: Data Clumps
aliases: []
tags:
- concept
summary: 一种代码异味（code smell），指多个变量总是同时一起出现，应打包成一个独立对象而不是分散传递。
created: '2026-08-26'
updated: '2026-08-26'
---

# Data Clumps

%% ytkb:def %%
一种代码异味（code smell），指多个变量总是同时一起出现，应打包成一个独立对象而不是分散传递。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-code-quality-design]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:aR97E7aKEgg %%
### 来自 [[2026-07-22-700-萬人下載的-grill-mematt-pocock-到底寫了什麼]]
- 如果买家姓名、电话、地址这几个变量总是绑在一起出现，就应该把它们打包成一个如「联络人」的物件，而不是每次都在代码里散着传来传去，这种现象叫做 Data Clumps。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[feature-envy]]
- [[jargon-as-compressed-instruction]]
- [[refactoring-book]]
%% ytkb:end %%
