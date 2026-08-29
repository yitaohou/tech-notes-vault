---
title: Plan-Execution Decoupling
aliases: []
tags:
- concept
summary: 为便于调试并防止模型执行不必要的 API 调用，将 agent 的规划阶段与执行阶段分离，先生成计划、验证后再执行的做法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Plan-Execution Decoupling

%% ytkb:def %%
为便于调试并防止模型执行不必要的 API 调用，将 agent 的规划阶段与执行阶段分离，先生成计划、验证后再执行的做法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 为便于调试并防止模型执行不必要的 API 调用，agent 的 planning 应与 execution 解耦：先让 agent 生成 plan，验证通过后才执行。（[39:04](https://youtu.be/JV3pL1_mn2M?t=2344)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[plan-validation-methods]]
%% ytkb:end %%
