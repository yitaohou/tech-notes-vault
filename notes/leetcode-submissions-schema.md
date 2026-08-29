---
title: LeetCode Submissions Table Schema
aliases: []
tags:
- concept
summary: 用于记录用户提交记录的表结构设计，字段包括 ID、competition ID、submitted 时间戳、test case result（通过/失败）、runtime
  和 error status。
created: '2026-08-26'
updated: '2026-08-26'
---

# LeetCode Submissions Table Schema

%% ytkb:def %%
用于记录用户提交记录的表结构设计，字段包括 ID、competition ID、submitted 时间戳、test case result（通过/失败）、runtime 和 error status。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- submissions 表的字段设计包括：ID、关联特定 contest 的 competition ID、提交时间戳、test case result（通过或失败）、代码运行所需的 runtime（秒），以及 error status。（[33:10](https://youtu.be/QBHTbtWSECg?t=1990)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[competition-id-partition-key]]
- [[leaderboard-as-derived-query]]
%% ytkb:end %%
