---
title: Planner Agent Tool Selection
aliases: []
tags:
- concept
summary: planner agent 根据当前任务需求，从可用工具列表中选择具体要调用的一个或多个工具组合来完成任务执行。
created: '2026-08-26'
updated: '2026-08-26'
---

# Planner Agent Tool Selection

%% ytkb:def %%
planner agent 根据当前任务需求，从可用工具列表中选择具体要调用的一个或多个工具组合来完成任务执行。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 针对退货场景，planner agent 会同时选择调用 Shopify 的退货 API 与 Stripe 的支付 API 这两个工具来完成任务。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[function-calling]]
- [[intent-specific-planner-agent]]
%% ytkb:end %%
