---
title: Requirement Scoping (Out of Scope)
aliases: []
tags:
- concept
summary: 通过显式声明某些功能为 out of scope（如 authentication、payment gateway）来缩小系统设计讨论范围、聚焦核心问题的技巧。
created: '2026-08-26'
updated: '2026-08-26'
---

# Requirement Scoping (Out of Scope)

%% ytkb:def %%
通过显式声明某些功能为 out of scope（如 authentication、payment gateway）来缩小系统设计讨论范围、聚焦核心问题的技巧。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-interview-methodology]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 设计 LeetCode 系统时，可以把 authorization、profile creation、payment gateway（用于 premium 服务）等功能显式列为 out of scope，从而把讨论精力集中在核心功能上。（[00:01](https://youtu.be/QBHTbtWSECg?t=1)）
%% ytkb:end %%

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 设计客服 agent 系统前应先明确功能范围，例如仅聚焦退货（returns）、换货（exchanges）和订单查询（where is my order），排除其他客服场景。（[00:00](https://youtu.be/CyLYY_xb5bQ?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-agent-automation-rate-target]]
- [[leetcode-core-functional-requirements]]
- [[system-design-functional-requirements-first]]
%% ytkb:end %%
