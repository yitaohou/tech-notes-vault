---
title: Meta-Agent / Feedback-Agent / Task-Agent Architecture
aliases: []
tags:
- concept
summary: 某些自我改进系统采用的三角色架构，包括负责生成策略的 meta-agent、负责评估反馈的 feedback-agent，以及负责实际执行任务的
  task-agent。
created: '2026-08-26'
updated: '2026-08-26'
---

# Meta-Agent / Feedback-Agent / Task-Agent Architecture

%% ytkb:def %%
某些自我改进系统采用的三角色架构，包括负责生成策略的 meta-agent、负责评估反馈的 feedback-agent，以及负责实际执行任务的 task-agent。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- 在某自我改进系统的实验中，task-agent 所用模型的能力强度远低于 meta-agent 和 feedback-agent，导致整体基线偏弱，结果难以与其他方法直接对比。（[21:11](https://youtu.be/z_F0z7wF5XU?t=1271)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[goodharts-law-objective-drift]]
%% ytkb:end %%
