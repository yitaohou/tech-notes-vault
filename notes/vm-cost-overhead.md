---
title: VM Cost Overhead
aliases: []
tags:
- concept
summary: VM 由于自带完整 operating system、比 container 更重量级，会带来更高的搭建与维护成本。
created: '2026-08-26'
updated: '2026-08-26'
---

# VM Cost Overhead

%% ytkb:def %%
VM 由于自带完整 operating system、比 container 更重量级，会带来更高的搭建与维护成本。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 选择 container 而非 VM 的一个原因是 VM 的维护成本更高，因为 VM 自带完整操作系统，比 container 更重。（[27:08](https://youtu.be/QBHTbtWSECg?t=1628)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[container-lightweight-architecture]]
- [[vm-resource-waste-per-instance]]
%% ytkb:end %%
