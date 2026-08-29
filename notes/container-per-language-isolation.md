---
title: Container Per Language Isolation
aliases: []
tags:
- concept
summary: 为每种编程语言分别分配一个独立的 container 来实现隔离执行的设计方式，常用于在线代码执行系统。
created: '2026-08-26'
updated: '2026-08-26'
---

# Container Per Language Isolation

%% ytkb:def %%
为每种编程语言分别分配一个独立的 container 来实现隔离执行的设计方式，常用于在线代码执行系统。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 针对代码执行系统中支持的每种编程语言，可以为其分配一个独立的 container 来实现隔离运行。（[27:08](https://youtu.be/QBHTbtWSECg?t=1628)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[docker-environment-consistency]]
- [[vm-container-isolation-tradeoff]]
%% ytkb:end %%
