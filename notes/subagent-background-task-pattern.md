---
title: Sub-Agent and Background Task Pattern (Harness Design Pattern)
aliases: []
tags:
- concept
summary: Harness设计的第三种模式：主agent生成多个子agent并行执行，同时监控后台任务状态，用于并行验证假设、跑实验或委派孤立子任务而不污染主上下文。
created: '2026-08-26'
updated: '2026-08-26'
---

# Sub-Agent and Background Task Pattern (Harness Design Pattern)

%% ytkb:def %%
Harness设计的第三种模式：主agent生成多个子agent并行执行，同时监控后台任务状态，用于并行验证假设、跑实验或委派孤立子任务而不污染主上下文。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- 当主 agent 需要同时验证多个假设、并行跑实验，或把孤立的子任务委派出去以避免污染主上下文时，子agent与后台任务模式非常有用。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[decentralized-multi-agent-architecture]]
- [[parallel-agent-execution]]
%% ytkb:end %%
