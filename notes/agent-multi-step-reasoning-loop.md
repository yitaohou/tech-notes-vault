---
title: Agent Multi-Step Reasoning Loop
aliases: []
tags:
- concept
summary: agent 执行复杂任务时典型的多步骤循环：推理如何完成任务、采取行动获取信息、评估信息是否充分、必要时重复行动，最终判断任务完成。
created: '2026-08-26'
updated: '2026-08-26'
---

# Agent Multi-Step Reasoning Loop

%% ytkb:def %%
agent 执行复杂任务时典型的多步骤循环：推理如何完成任务、采取行动获取信息、评估信息是否充分、必要时重复行动，最终判断任务完成。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 以预测未来三个月销售收入为例，agent 会先推理如何完成任务，生成 SQL 查询获取历史销售数据，执行查询后分析信息是否充分，必要时再生成并执行额外查询，最后基于收集到的数据做出预测并判断任务已完成。（[36:03](https://youtu.be/JV3pL1_mn2M?t=2163)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-definition]]
- [[text-to-sql-rag]]
%% ytkb:end %%
