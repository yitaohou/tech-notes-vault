---
title: DeepSeek Harness Batch Script Mode
aliases: []
tags:
- concept
summary: DeepSeek Harness 的一种运行模式，让模型直接写一段程序、把多个工具操作合并成一次执行完成，用于节省 token 消耗。
created: '2026-09-03'
updated: '2026-09-04'
---

# DeepSeek Harness Batch Script Mode

%% ytkb:def %%
DeepSeek Harness 的一种运行模式，让模型直接写一段程序、把多个工具操作合并成一次执行完成，用于节省 token 消耗。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 该模式通过让模型编写脚本一次性完成多步工具调用，减少多轮交互带来的 token 消耗。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
%% ytkb:end %%

%% ytkb:video:buYQ-_V2Wv0 %%
### 来自 [[2026-09-04-一个视频搞懂deepseek-harness]]
- PTC 模式下模型会把要用到的多个工具调用一次性写进一个脚本执行，而不是每用一次工具就停下来思考一次，从而更省时间和 token。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- 批处理执行工具调用能减少模型的思考步骤数量，使模型不容易从高水平的思维链推理退化回逐步试探的低效模式。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-harness]]
- [[deepseek-harness-creative-mode]]
- [[deepseek-harness-mechanical-mode]]
- [[deepseek-harness-modes]]
%% ytkb:end %%
