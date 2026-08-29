---
title: Eventual Consistency for Submission Feedback
aliases: []
tags:
- concept
summary: 允许代码提交后各测试用例的即时反馈结果存在延迟或跨节点不一致，但要求服务本身始终保持可用的具体设计取舍。
created: '2026-08-26'
updated: '2026-08-26'
---

# Eventual Consistency for Submission Feedback

%% ytkb:def %%
允许代码提交后各测试用例的即时反馈结果存在延迟或跨节点不一致，但要求服务本身始终保持可用的具体设计取舍。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 在 LeetCode 系统设计中，代码提交后拿到全部测试用例的即时反馈可以有延迟（eventual consistency），但服务本身不能宕机——保持系统可用比让所有节点对同一提交结果立刻达成一致更重要。（[03:01](https://youtu.be/QBHTbtWSECg?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[availability-over-consistency-tradeoff]]
- [[low-latency-response-time-requirement]]
%% ytkb:end %%
