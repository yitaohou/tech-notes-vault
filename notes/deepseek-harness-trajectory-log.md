---
title: DeepSeek Harness Trajectory Log
aliases: []
tags:
- concept
summary: DeepSeek Harness 的安全设计之一，以 append-only 方式完整记录 AI 每轮交互中看到的内容、推理过程、调用的工具及返回结果。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Trajectory Log

%% ytkb:def %%
DeepSeek Harness 的安全设计之一，以 append-only 方式完整记录 AI 每轮交互中看到的内容、推理过程、调用的工具及返回结果。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 轨迹日志采用 append-only 特性，只能往里追加内容而不能修改或删除已写入的记录，确保模型历史行为可完整追溯。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- DeepSeek Harness的轨迹日志会按顺序记住每一轮交互的五样东西：用户发了什么、模型看到什么、模型做了什么推理、调用了什么工具、工具返回了什么结果，从而完整回答AI到底做了什么。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-harness]]
- [[ai-system-observability]]
- [[trajectory-log-append-only]]
- [[trajectory-log-storage-location]]
%% ytkb:end %%
