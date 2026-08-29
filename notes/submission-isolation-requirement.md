---
title: Submission Isolation Requirement
aliases: []
tags:
- concept
summary: 要求每份代码提交的执行相互隔离，一份提交的运行不能干扰或影响其他提交及系统整体稳定性的系统设计需求。
created: '2026-08-26'
updated: '2026-08-26'
---

# Submission Isolation Requirement

%% ytkb:def %%
要求每份代码提交的执行相互隔离，一份提交的运行不能干扰或影响其他提交及系统整体稳定性的系统设计需求。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 系统需要保证每个用户提交的代码在运行测试用例时彼此隔离，不会互相干扰，也不会影响当前系统的稳定性。（[06:02](https://youtu.be/QBHTbtWSECg?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[code-execution-sandboxing]]
%% ytkb:end %%
