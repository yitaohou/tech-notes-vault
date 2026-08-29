---
title: Execution Timeout Limit
aliases: []
tags:
- concept
summary: 对用户提交代码的执行设置超时上限（如2秒或5秒），超时即判定为TLE并终止执行，用于防止死循环并提升运行用户代码的安全性。
created: '2026-08-26'
updated: '2026-08-26'
---

# Execution Timeout Limit

%% ytkb:def %%
对用户提交代码的执行设置超时上限（如2秒或5秒），超时即判定为TLE并终止执行，用于防止死循环并提升运行用户代码的安全性。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-security]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 为防止用户提交的代码出现死循环，可以对代码执行设置超时上限（如2秒或5秒），一旦超过该时限就终止执行（TLE），从而阻止无限循环并进一步保障运行用户代码的安全性。（[39:13](https://youtu.be/QBHTbtWSECg?t=2353)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[isolated-execution-environment]]
%% ytkb:end %%
