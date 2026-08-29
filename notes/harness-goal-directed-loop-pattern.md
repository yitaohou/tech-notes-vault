---
title: Goal-Directed Loop Pattern (Harness Design Pattern)
aliases: []
tags:
- concept
summary: Harness设计的第一种通用模式：先做计划、再执行、然后观察结果或测试效果，接着根据反馈改进并进入下一轮，直到达成目标。
created: '2026-08-26'
updated: '2026-08-26'
---

# Goal-Directed Loop Pattern (Harness Design Pattern)

%% ytkb:def %%
Harness设计的第一种通用模式：先做计划、再执行、然后观察结果或测试效果，接着根据反馈改进并进入下一轮，直到达成目标。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- 与静态提示词模板不同，目标导向循环模式更强调模型在运行时持续分析自己的执行轨迹和失败案例，一步步迭代推进任务。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
- 在目标导向循环执行过程中，如果任务描述不清晰或执行偏好不明确，agent 可以主动向用户确认，而不是自行猜测。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-harness]]
- [[agent-multi-step-reasoning-loop]]
- [[ai-blind-spot-questioning]]
%% ytkb:end %%
