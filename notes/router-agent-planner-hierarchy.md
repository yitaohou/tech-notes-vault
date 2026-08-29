---
title: Router Agent to Specialized Planner Hierarchy
aliases: []
tags:
- concept
summary: router agent 位于系统较高层级，负责决定将用户请求路由到具体的专业 planner agent（如 return planner、exchange
  planner、order status agent）。
created: '2026-08-26'
updated: '2026-08-26'
---

# Router Agent to Specialized Planner Hierarchy

%% ytkb:def %%
router agent 位于系统较高层级，负责决定将用户请求路由到具体的专业 planner agent（如 return planner、exchange planner、order status agent）。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- router agent 处于比各专业 planner agent 更高的层级，其职责是判断应该把当前请求路由给哪个具体的 planner（如退货、换货或订单查询）。（[15:04](https://youtu.be/CyLYY_xb5bQ?t=904)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[centralized-agent-architecture]]
- [[qa-agent-central-hub-role]]
%% ytkb:end %%
