---
title: Intent-Specific Planner Agent
aliases: []
tags:
- concept
summary: 根据 router agent 识别出的具体用户意图，系统调用与该意图对应的专门 planner agent（例如退货意图对应 return planning
  agent）来处理后续步骤。
created: '2026-08-26'
updated: '2026-08-26'
---

# Intent-Specific Planner Agent

%% ytkb:def %%
根据 router agent 识别出的具体用户意图，系统调用与该意图对应的专门 planner agent（例如退货意图对应 return planning agent）来处理后续步骤。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 当 router agent 判定用户意图为退货时，会调用专门的 return planning agent 接手处理后续的退货流程规划。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[model-routing]]
%% ytkb:end %%
