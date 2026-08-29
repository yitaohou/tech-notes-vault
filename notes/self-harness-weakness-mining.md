---
title: Self-Harness 弱点挖掘阶段
aliases: []
tags:
- concept
summary: Self-Harness 的第一阶段，把任务运行中的失败案例聚类成基于验证器的失败模式，用于定位真正的改进方向。
created: '2026-08-26'
updated: '2026-08-26'
---

# Self-Harness 弱点挖掘阶段

%% ytkb:def %%
Self-Harness 的第一阶段，把任务运行中的失败案例聚类成基于验证器的失败模式，用于定位真正的改进方向。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- 弱点挖掘阶段的失败记录需要包含验证层原因、相关 Agent 行为的因果状态、轨迹暴露的抽象机制等丰富信息，因为表面相同的错误（如超时或缺少产物）背后的因果机制可能完全不同，只有信息足够丰富才能挖到根因。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[self-harness]]
%% ytkb:end %%
