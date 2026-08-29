---
title: Low Latency Requirement for Judge System
aliases: []
tags:
- concept
summary: 判题系统的非功能性需求之一，要求提交代码后的执行结果能在较短时间阈值内返回。
created: '2026-08-26'
updated: '2026-08-26'
---

# Low Latency Requirement for Judge System

%% ytkb:def %%
判题系统的非功能性需求之一，要求提交代码后的执行结果能在较短时间阈值内返回。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 判题系统需要满足低延迟要求，例如把提交结果返回时间限制在类似 2 秒或 5 秒以内，具体阈值留待后续讨论确定。（[06:02](https://youtu.be/QBHTbtWSECg?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[time-limit-exceeded-handling]]
%% ytkb:end %%
