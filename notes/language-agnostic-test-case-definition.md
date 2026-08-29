---
title: Language-Agnostic Test Case Definition
aliases: []
tags:
- concept
summary: 跨编程语言判题系统中，用与具体语言实现无关的元数据来描述测试用例输入输出，使同一套测试逻辑可在不同语言间复用的设计。
created: '2026-08-26'
updated: '2026-08-26'
---

# Language-Agnostic Test Case Definition

%% ytkb:def %%
跨编程语言判题系统中，用与具体语言实现无关的元数据来描述测试用例输入输出，使同一套测试逻辑可在不同语言间复用的设计。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 尽管同一道题在不同编程语言下的数据结构实现不同（如 Java 和 Python 的树结构对象不同），跨语言判题系统仍可为每道题设计统一的测试用例定义，用与语言无关的元数据描述输入输出，从而在不同语言间复用同一套测试逻辑。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[per-language-runtime-containers]]
%% ytkb:end %%
