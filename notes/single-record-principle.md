---
title: Single Record Principle
aliases: []
tags:
- concept
summary: 前端 state 架构原则：同一份数据在整个状态体系中只应被表示一次，不允许重复存储。
created: '2026-08-26'
updated: '2026-08-26'
---

# Single Record Principle

%% ytkb:def %%
前端 state 架构原则：同一份数据在整个状态体系中只应被表示一次，不允许重复存储。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-state-management]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 为约束 AI 生成的 state 架构，需要明确要求其遵循 single record principle：一份数据在整个状态中只表示一次。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
%% ytkb:end %%

%% ytkb:video:hA_XnzB1Ef8 %%
### 来自 [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof]]
- essential state 设计应遵循 single record principle：系统中任何一份数据都必须只被存储一次，不能有冗余状态，也不能有可以从其他状态推导出来的 derived state，state 应尽量最小化。（[12:03](https://youtu.be/hA_XnzB1Ef8?t=723)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[essential-state]]
- [[state-duplication-performance-risk]]
%% ytkb:end %%
