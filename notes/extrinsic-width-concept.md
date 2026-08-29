---
title: Extrinsic Width
aliases: []
tags:
- concept
summary: extrinsic width 指开发者显式指定的宽度值，其含义随 box-sizing 设置不同而不同：在 border-box 下代表包含 padding
  和 border 的总宽度，在 content-box（默认）下浏览器会另外计算并叠加 padding 和 border。
created: '2026-08-26'
updated: '2026-08-26'
---

# Extrinsic Width

%% ytkb:def %%
extrinsic width 指开发者显式指定的宽度值，其含义随 box-sizing 设置不同而不同：在 border-box 下代表包含 padding 和 border 的总宽度，在 content-box（默认）下浏览器会另外计算并叠加 padding 和 border。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-css-styling]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 当元素设为 border-box 并指定 width: 300px 时，浏览器会把这个值当作固定总宽度去挤压内容，内容过多则产生溢出（overflow）。（[21:06](https://youtu.be/AMerB8XjfZ0?t=1266)）
- 在默认的 content-box 模式下，浏览器会先计算内容本身所需的宽度，再自动叠加你设置的 padding，而不是把指定宽度当作总宽度。（[21:06](https://youtu.be/AMerB8XjfZ0?t=1266)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[css-box-sizing-property]]
%% ytkb:end %%
