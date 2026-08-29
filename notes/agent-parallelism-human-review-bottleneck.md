---
title: Human Review as the Real Bottleneck for Agent Parallelism
aliases: []
tags:
- concept
summary: 工作树只解决了机械层面的文件冲突，但整个流程真正的瓶颈是人能认真审核多少代码产出，这一限制被称为编排税（coordination tax）。
created: '2026-08-26'
updated: '2026-08-26'
---

# Human Review as the Real Bottleneck for Agent Parallelism

%% ytkb:def %%
工作树只解决了机械层面的文件冲突，但整个流程真正的瓶颈是人能认真审核多少代码产出，这一限制被称为编排税（coordination tax）。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 工作树解决的只是机械层面的文件冲突，整个流程的瓶颈依然是人本身：一个人一天能认真审核多少份代码产出，才是实际能并行运行多少Agent的上限，而不是工具能同时跑多少线程，这被称为编排税。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[coordination-tax-multi-agent]]
- [[git-worktree-multi-agent-isolation]]
%% ytkb:end %%
