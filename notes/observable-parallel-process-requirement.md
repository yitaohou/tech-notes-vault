---
title: Observable Parallel Process Requirement
aliases: []
tags:
- concept
summary: 子agent并行执行设计中的关键要求：并行过程必须明确可观测，即输出需持久化为文件、日志或状态记录，而非只存在临时聊天上下文中。
created: '2026-08-26'
updated: '2026-08-26'
---

# Observable Parallel Process Requirement

%% ytkb:def %%
子agent并行执行设计中的关键要求：并行过程必须明确可观测，即输出需持久化为文件、日志或状态记录，而非只存在临时聊天上下文中。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- 如果子agent的输出只存在临时的聊天上下文里，很快就会失效且无法追溯；但如果都存成文件、日志、状态记录，模型即使中途被打断也能恢复，还能基于完整执行历史做推理。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[file-system-persistent-memory]]
- [[subagent-background-task-pattern]]
%% ytkb:end %%
