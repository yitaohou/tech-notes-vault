---
title: Model Routing by Task Complexity
aliases:
- Using Cheaper Models for Simple Subtasks
tags:
- concept
summary: 根据任务复杂度将请求分流给不同规模模型的工程实践：简单任务用小模型，复杂长程推理任务用顶配模型。
created: '2026-08-26'
updated: '2026-08-26'
---

# Model Routing by Task Complexity

%% ytkb:def %%
根据任务复杂度将请求分流给不同规模模型的工程实践：简单任务用小模型，复杂长程推理任务用顶配模型。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-model-selection-deployment]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- 工程上常见做法是按任务复杂度分流：简单补全和基础问答用小模型，只有跨多文件、需要长程推理的硬核重构才调用顶配模型。（[09:02](https://youtu.be/Lle_EJljIoo?t=542)）
- 模型分流并非官方规定的固定架构，而是一种通用的成本控制思路，具体如何分流需要根据自身业务量来调整。（[09:02](https://youtu.be/Lle_EJljIoo?t=542)）
%% ytkb:end %%

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 任务被拆分成子任务后，可以为较简单的步骤单独使用更便宜的模型来降低整体成本。（[27:02](https://youtu.be/JV3pL1_mn2M?t=1622)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[decompose-complex-tasks-prompting]]
%% ytkb:end %%
