---
title: Open-Box Rule Display Order vs Hit Order
aliases: []
tags:
- concept
summary: Open-Box 中规则集在界面上的显示排序与规则实际命中判定的顺序是两个独立机制，调整显示排序不会影响真实命中顺序。
created: '2026-09-08'
updated: '2026-09-08'
---

# Open-Box Rule Display Order vs Hit Order

%% ytkb:def %%
Open-Box 中规则集在界面上的显示排序与规则实际命中判定的顺序是两个独立机制，调整显示排序不会影响真实命中顺序。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-software-router-tools]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:G_7AmjfSRQ8 %%
### 来自 [[2026-09-07-最新软路由代理-open-box-发布全图形极简配置超越-openclashnikkipasswal]]
- 在设置窗口里可以单独调整规则集的显示排序（例如把某条规则拖到列表下方以避免显得突兀），但这只影响界面展示顺序，右侧实际命中规则的判定顺序并不会因此改变。（[21:08](https://youtu.be/G_7AmjfSRQ8?t=1268)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[openbox-rule-top-down-matching]]
%% ytkb:end %%
