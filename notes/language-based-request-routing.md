---
title: Language-Based Submission Routing
aliases: []
tags:
- concept
summary: 针对某个 problem，用户提交的代码依据其编程语言被路由到对应语言 runtime 容器处理的机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# Language-Based Submission Routing

%% ytkb:def %%
针对某个 problem，用户提交的代码依据其编程语言被路由到对应语言 runtime 容器处理的机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 用户针对某个 problem 提交代码时，系统会依据所用编程语言把相关请求路由到该语言对应的 runtime 容器进行处理。（[30:08](https://youtu.be/QBHTbtWSECg?t=1808)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[container-per-language-runtime]]
%% ytkb:end %%
