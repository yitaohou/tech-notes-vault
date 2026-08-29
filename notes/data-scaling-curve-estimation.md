---
title: Data Scaling Curve Estimation
aliases: []
tags:
- concept
summary: 用当前数据集的 25%、50%、100% 等子集分别训练模型、观察性能变化趋势，从而估计还需要多少数据的方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Data Scaling Curve Estimation

%% ytkb:def %%
用当前数据集的 25%、50%、100% 等子集分别训练模型、观察性能变化趋势，从而估计还需要多少数据的方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-training-data]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 若训练效果随数据集增大持续陡峭上升，说明扩大数据集能带来显著提升；若表现趋于平台期，则说明继续加数据收益递减。（[57:04](https://youtu.be/JV3pL1_mn2M?t=3424)）
%% ytkb:end %%
