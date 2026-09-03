---
title: Trajectory Three-Tier Learning Routing
aliases: []
tags:
- concept
summary: Trajectory 提出的将捕捉到的经验按性质分流到模型权重、上下文/记忆、工具/Harness三个不同层级分别处理的机制。
created: '2026-09-02'
updated: '2026-09-02'
---

# Trajectory Three-Tier Learning Routing

%% ytkb:def %%
Trajectory 提出的将捕捉到的经验按性质分流到模型权重、上下文/记忆、工具/Harness三个不同层级分别处理的机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-continual-learning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:zyzeyxuG42Q %%
### 来自 [[2026-08-19-下一代大模型持续学习]]
- Trajectory 把捕捉到的经验分成三层处理：全局通用规律（如某工具调用总是失败）训练进模型权重让所有用户受益；用户个人偏好（如不想用某个Agent）放入上下文或记忆；具体事实性信息（如某公司退市、财报数据）放在工具/Harness层处理。（[03:00](https://youtu.be/zyzeyxuG42Q?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[memory-tier-routing-os-analogy]]
- [[trajectory-continual-learning-system]]
%% ytkb:end %%
