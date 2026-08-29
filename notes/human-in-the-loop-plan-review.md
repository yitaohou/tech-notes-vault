---
title: Human-in-the-Loop Plan Review
aliases: []
tags:
- concept
summary: 在执行前引入人工审查 agent 生成计划的机制，常用于重要或敏感任务。
created: '2026-08-26'
updated: '2026-08-26'
---

# Human-in-the-Loop Plan Review

%% ytkb:def %%
在执行前引入人工审查 agent 生成计划的机制，常用于重要或敏感任务。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 对于特别重要或敏感的任务，可以在执行前引入人工审查 agent 生成的 plan，即 human in the loop。（[39:04](https://youtu.be/JV3pL1_mn2M?t=2344)）
%% ytkb:end %%

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 在多 agent 客服系统中，可在 router agent 判断请求有效后插入人工审批环节，由人类决定是否批准该请求，以保障整体客户满意度不受影响。（[09:01](https://youtu.be/CyLYY_xb5bQ?t=541)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[router-agent-policy-check]]
%% ytkb:end %%
