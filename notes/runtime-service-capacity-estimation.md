---
title: Runtime Service Capacity Estimation
aliases: []
tags:
- concept
summary: 根据预期用户规模来估算需要部署多少个 runtime service 实例的容量规划方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Runtime Service Capacity Estimation

%% ytkb:def %%
根据预期用户规模来估算需要部署多少个 runtime service 实例的容量规划方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-scalability]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 对于面向百万级用户的在线代码执行服务，大约三四台 runtime server 即可支撑负载，具体数字应基于实际业务量做更精确的估算。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[horizontal-scaling]]
%% ytkb:end %%
