---
title: Separate Verifier Agent for Goal Completion
aliases: []
tags:
- concept
summary: 在目标导向的循环执行模式中，用一个独立于写代码Agent的小模型，在每轮结束后专门检查目标是否已经完成。
created: '2026-08-26'
updated: '2026-08-26'
---

# Separate Verifier Agent for Goal Completion

%% ytkb:def %%
在目标导向的循环执行模式中，用一个独立于写代码Agent的小模型，在每轮结束后专门检查目标是否已经完成。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 在/goal 模式下，每轮执行结束后由一个独立的小模型检查目标是否完成，写代码的Agent与判断任务是否完成的Agent是两个不同的Agent。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[goal-directed-persistent-loop]]
%% ytkb:end %%
