---
title: Separate Model for Loop Completion Check
aliases: []
tags:
- concept
summary: 用一个独立于执行任务的全新模型来判断循环或任务是否完成，把生成与校验分离的逻辑应用到停止条件判断上的设计。
created: '2026-08-26'
updated: '2026-08-26'
---

# Separate Model for Loop Completion Check

%% ytkb:def %%
用一个独立于执行任务的全新模型来判断循环或任务是否完成，把生成与校验分离的逻辑应用到停止条件判断上的设计。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- /goal 指令底层用的也是生成与校验分离的逻辑：判断循环有没有完成的是一个全新的模型，而不是执行任务的那个模型。（[13:10](https://youtu.be/KgiwIEBeOHw?t=790)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-judge]]
- [[unattended-loop-trusted-verification]]
%% ytkb:end %%
