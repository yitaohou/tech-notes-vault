---
title: Container-Per-Language Runtime Design
aliases: []
tags:
- concept
summary: 代码执行系统中按编程语言划分容器（如一个 Python 容器、一个 Java 容器），容器内并发运行多个提交任务以避免资源浪费的设计。
created: '2026-08-26'
updated: '2026-08-26'
---

# Container-Per-Language Runtime Design

%% ytkb:def %%
代码执行系统中按编程语言划分容器（如一个 Python 容器、一个 Java 容器），容器内并发运行多个提交任务以避免资源浪费的设计。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 为避免每个用户提交都单独占用一个容器造成资源浪费，设计上按语言划分容器（如一个容器跑 Python、一个容器跑 Java），并在同一容器内同时运行多个提交或结果校验任务。（[30:08](https://youtu.be/QBHTbtWSECg?t=1808)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[container-shared-kernel-isolation]]
- [[nested-runtime-scoping]]
%% ytkb:end %%
