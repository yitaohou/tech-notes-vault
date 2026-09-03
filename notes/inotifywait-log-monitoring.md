---
title: Inotifywait Log Monitoring
aliases: []
tags:
- concept
summary: 用inotifywait等文件监听工具挂载在轨迹日志文件上，日志一旦有新增内容就自动触发检查的自动化监控方式。
created: '2026-09-03'
updated: '2026-09-03'
---

# Inotifywait Log Monitoring

%% ytkb:def %%
用inotifywait等文件监听工具挂载在轨迹日志文件上，日志一旦有新增内容就自动触发检查的自动化监控方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 如果想更省事，可以用inotifywait这类文件监听工具挂在日志文件上，日志一有追加就自动触发检查，不用自己记着定期手动跑命令。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[grep-periodic-monitoring]]
%% ytkb:end %%
