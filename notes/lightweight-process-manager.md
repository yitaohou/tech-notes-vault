---
title: Lightweight Process Manager for Sub-Agents
aliases: []
tags:
- concept
summary: 主 agent 在子agent和后台任务模式中用来启动任务、查看日志、取消失败运行、并把结果合并回主线程的轻量级进程管理组件。
created: '2026-08-26'
updated: '2026-08-26'
---

# Lightweight Process Manager for Sub-Agents

%% ytkb:def %%
主 agent 在子agent和后台任务模式中用来启动任务、查看日志、取消失败运行、并把结果合并回主线程的轻量级进程管理组件。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- 在子agent与后台任务模式中，主agent需要一个轻量的进程管理器，负责启动任务、查看日志、取消失败的运行，最后把结果合并回主线程。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[subagent-background-task-pattern]]
%% ytkb:end %%
