---
title: AFlow
aliases: []
tags:
- concept
summary: 把 agent 工作流表示成图（节点为调用大模型的动作，边为代码实现的逻辑操作），并用 Monte Carlo Tree Search 优化工作流的方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# AFlow

%% ytkb:def %%
把 agent 工作流表示成图（节点为调用大模型的动作，边为代码实现的逻辑操作），并用 Monte Carlo Tree Search 优化工作流的方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- AFlow 从初始工作流模板出发，每轮按分数与探索的混合策略选择一个节点，让大模型根据评估结果修改生成新工作流，执行评估后有提升的工作流加回搜索树，直到分数平稳或用完计算预算。（[12:08](https://youtu.be/z_F0z7wF5XU?t=728)）
- 实验显示，在问答、代码、数学等任务上，AFlow 的表现比人工设计的工作流和 ADAS 都要好不少。（[12:08](https://youtu.be/z_F0z7wF5XU?t=728)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ads-automated-design-agentic-systems]]
- [[agentic-workflow-design-as-search-problem]]
%% ytkb:end %%
