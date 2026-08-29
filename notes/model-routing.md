---
title: Model Routing
aliases: []
tags:
- concept
summary: 根据用户意图将query分流到不同模型或pipeline的机制，通常由一个intent classifier驱动。
created: '2026-08-26'
updated: '2026-08-26'
---

# Model Routing

%% ytkb:def %%
根据用户意图将query分流到不同模型或pipeline的机制，通常由一个intent classifier驱动。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-model-selection-deployment]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- model router通常包含一个intent classifier，用于预测用户意图，再据此把query导向合适的模型或pipeline。（[69:07](https://youtu.be/JV3pL1_mn2M?t=4147)）
%% ytkb:end %%

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- router agent 的核心职责是识别用户请求的意图（如「退货」），并据此将请求分流给对应的下游 planner agent 处理。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[intent-specific-planner-agent]]
- [[model-gateway]]
- [[model-router-latency-cost-requirement]]
%% ytkb:end %%
