---
title: Code Template Selection by Language
aliases: []
tags:
- concept
summary: 在代码提交类系统设计中，用户选择编程语言后，系统需要提供该语言对应的函数模板（如 formatter client、template client、compiler
  client）。
created: '2026-08-26'
updated: '2026-08-26'
---

# Code Template Selection by Language

%% ytkb:def %%
在代码提交类系统设计中，用户选择编程语言后，系统需要提供该语言对应的函数模板（如 formatter client、template client、compiler client）。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 当用户选择编程语言（如 Python）后，系统需要提供该语言对应的函数模板，涉及 formatter client、template client 和 compiler client 等组件。（[18:07](https://youtu.be/QBHTbtWSECg?t=1087)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[submit-problem-api-design]]
%% ytkb:end %%
