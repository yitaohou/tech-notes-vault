---
title: VM Resource Waste Per Instance
aliases: []
tags:
- concept
summary: 在系统设计中，每个 VM 都拥有自己独立的内存和计算资源，多个 VM 并存会造成计算资源的浪费。
created: '2026-08-26'
updated: '2026-08-26'
---

# VM Resource Waste Per Instance

%% ytkb:def %%
在系统设计中，每个 VM 都拥有自己独立的内存和计算资源，多个 VM 并存会造成计算资源的浪费。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 采用 VM-based 架构为每个执行环境分配独立的内存和计算资源，属于对计算资源的低效使用。（[27:08](https://youtu.be/QBHTbtWSECg?t=1628)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[container-lightweight-architecture]]
- [[vm-cost-overhead]]
%% ytkb:end %%
