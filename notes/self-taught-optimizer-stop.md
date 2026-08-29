---
title: Self-Taught Optimizer (STOP)
aliases: []
tags:
- concept
summary: 递归脚手架改进的早期代表性工作，初始优化器接收一个解决方案、一个效用函数和一个黑盒大模型，返回改进后的解决方案，但其目标是改进优化器本身而非具体解。
created: '2026-08-26'
updated: '2026-08-26'
---

# Self-Taught Optimizer (STOP)

%% ytkb:def %%
递归脚手架改进的早期代表性工作，初始优化器接收一个解决方案、一个效用函数和一个黑盒大模型，返回改进后的解决方案，但其目标是改进优化器本身而非具体解。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- STOP 定义了「元效用（meta-utility）」——优化器在一系列下游任务上的平均效用——并通过递归方式用上一代优化器优化自身，生成下一代优化器。（[12:08](https://youtu.be/z_F0z7wF5XU?t=728)）
- 实验中，自我改进后的优化器自主发现了多种优化策略，包括遗传算法、分部分改进、多臂老虎机提示词、模拟退火、调整采样温度、波束搜索和树搜索等。（[12:08](https://youtu.be/z_F0z7wF5XU?t=728)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[harness-as-code]]
%% ytkb:end %%
