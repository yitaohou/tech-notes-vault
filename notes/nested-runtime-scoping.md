---
title: Nested Language/Process Runtime Scoping
aliases: []
tags:
- concept
summary: 代码执行系统中在语言级 runtime 容器内部再按每个 problem 划分出 process 级 runtime 的两层作用域隔离设计。
created: '2026-08-26'
updated: '2026-08-26'
---

# Nested Language/Process Runtime Scoping

%% ytkb:def %%
代码执行系统中在语言级 runtime 容器内部再按每个 problem 划分出 process 级 runtime 的两层作用域隔离设计。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 语言级 runtime 容器内部还可以进一步按每个 problem 划出独立的 process 级 runtime 作用域，实现语言层和进程层的两层隔离划分。（[30:08](https://youtu.be/QBHTbtWSECg?t=1808)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[container-per-language-runtime]]
- [[language-based-request-routing]]
%% ytkb:end %%
