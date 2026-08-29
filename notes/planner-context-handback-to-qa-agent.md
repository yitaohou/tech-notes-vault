---
title: Planner Agent Context Handback Pattern
aliases: []
tags:
- concept
summary: 各专业 planner agent（如 return planner、exchange planner）完成任务后，必须把最新上下文和结果状态回传给
  Q&A agent，由后者负责与用户实时沟通。
created: '2026-08-26'
updated: '2026-08-26'
---

# Planner Agent Context Handback Pattern

%% ytkb:def %%
各专业 planner agent（如 return planner、exchange planner）完成任务后，必须把最新上下文和结果状态回传给 Q&A agent，由后者负责与用户实时沟通。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 无论任务成功还是失败（例如商品或问题不符合退货政策），planner agent 完成处理后都要把最新状态更新回 Q&A agent，以便 Q&A agent 能实时回应用户。（[15:04](https://youtu.be/CyLYY_xb5bQ?t=904)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[qa-agent-central-hub-role]]
%% ytkb:end %%
