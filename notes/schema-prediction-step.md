---
title: Schema Prediction Step
aliases: []
tags:
- concept
summary: 在 text-to-SQL 场景中，当数据库表过多、无法把所有表结构塞进上下文窗口时，先预测应使用哪张表的中间步骤。
created: '2026-08-26'
updated: '2026-08-26'
---

# Schema Prediction Step

%% ytkb:def %%
在 text-to-SQL 场景中，当数据库表过多、无法把所有表结构塞进上下文窗口时，先预测应使用哪张表的中间步骤。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 对于表结构复杂、表数量过多以至无法把所有 schema 都放入上下文窗口的数据库，text-to-SQL 流程可能需要增加一个中间步骤，先预测每次查询该使用哪张表。（[36:03](https://youtu.be/JV3pL1_mn2M?t=2163)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[context-window-limits-large-models]]
- [[text-to-sql-rag]]
%% ytkb:end %%
