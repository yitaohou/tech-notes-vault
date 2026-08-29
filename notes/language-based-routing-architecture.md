---
title: Language-Based Routing Architecture
aliases: []
tags:
- concept
summary: 系统架构中按编程语言将代码执行请求路由到对应专用服务器或节点的设计思路。
created: '2026-08-26'
updated: '2026-08-26'
---

# Language-Based Routing Architecture

%% ytkb:def %%
系统架构中按编程语言将代码执行请求路由到对应专用服务器或节点的设计思路。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 语言过滤的核心原因是：系统需要知道该把请求路由到哪个语言专属的编译节点或服务器去执行，因为不同语言通常对应不同的执行节点。（[15:06](https://youtu.be/QBHTbtWSECg?t=906)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[language-filter-problem-submission]]
- [[problem-supports-multiple-languages]]
%% ytkb:end %%
