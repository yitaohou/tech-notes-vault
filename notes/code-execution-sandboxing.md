---
title: Code Execution Sandboxing
aliases: []
tags:
- concept
summary: 在判题类系统（如 LeetCode）中为运行用户提交代码而设置的隔离执行环境，防止恶意代码影响整体服务。
created: '2026-08-26'
updated: '2026-08-26'
---

# Code Execution Sandboxing

%% ytkb:def %%
在判题类系统（如 LeetCode）中为运行用户提交代码而设置的隔离执行环境，防止恶意代码影响整体服务。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 用户提交的代码可能包含 malware，如果不加隔离运行，可能导致整个 judge 服务被攻击者拖垮。（[06:02](https://youtu.be/QBHTbtWSECg?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[submission-isolation-requirement]]
%% ytkb:end %%
