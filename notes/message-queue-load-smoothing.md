---
title: Message Queue for Load Smoothing
aliases: []
tags:
- concept
summary: 在 API server 与执行容器之间引入消息队列，用以更好地路由请求并平滑流量高峰的架构手段。
created: '2026-08-26'
updated: '2026-08-26'
---

# Message Queue for Load Smoothing

%% ytkb:def %%
在 API server 与执行容器之间引入消息队列，用以更好地路由请求并平滑流量高峰的架构手段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-communication-patterns]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 在 API server 与代码执行容器之间引入 message queue，可以更好地路由请求并平滑突发流量高峰，避免容器直接承受流量冲击。（[42:13](https://youtu.be/QBHTbtWSECg?t=2533)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[horizontal-scaling]]
- [[worker-pull-pattern]]
%% ytkb:end %%
