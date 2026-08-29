---
title: Exponential Backoff Retry
aliases: []
tags:
- concept
summary: 失败重试时让重试间隔随失败次数增加而逐渐变长的重试策略。
created: '2026-08-26'
updated: '2026-08-26'
---

# Exponential Backoff Retry

%% ytkb:def %%
失败重试时让重试间隔随失败次数增加而逐渐变长的重试策略。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-messaging-queues]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 当代码执行容器处理某次提交失败时，可以引入指数退避重试机制，即每次失败后的重试等待时间随重试次数增加而变长。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
%% ytkb:end %%
