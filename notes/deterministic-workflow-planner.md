---
title: Deterministic Workflow Planner
aliases: []
tags:
- concept
summary: 当任务流程高度固定时，planner agent 可以不依赖大模型自主推理，而是采用基于规则的确定性工作流（deterministic workflow）来完成任务执行。
created: '2026-08-26'
updated: '2026-08-26'
---

# Deterministic Workflow Planner

%% ytkb:def %%
当任务流程高度固定时，planner agent 可以不依赖大模型自主推理，而是采用基于规则的确定性工作流（deterministic workflow）来完成任务执行。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 对于流程非常固定的任务（如标准退货流程：先判断商品是否符合退货条件，再触发 Stripe 处理退款），可以用确定性规则工作流代替 agent 自主推理，以提升可控性。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[intent-specific-planner-agent]]
- [[planner-agent-tool-selection]]
%% ytkb:end %%
