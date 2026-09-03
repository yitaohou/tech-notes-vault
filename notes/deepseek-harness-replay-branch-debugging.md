---
title: DeepSeek Harness Replay and Branch Debugging
aliases: []
tags:
- concept
summary: 基于 append-only 轨迹日志实现的调试能力，出事后可完整回放模型行为，还能从任意历史节点创建分支重新运行以比较不同选择的结果。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Replay and Branch Debugging

%% ytkb:def %%
基于 append-only 轨迹日志实现的调试能力，出事后可完整回放模型行为，还能从任意历史节点创建分支重新运行以比较不同选择的结果。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 相比其他 agent 出事后只能靠猜测或依赖有限上下文分析报错，DeepSeek Harness 能像回放录像一样完整重现整个交互过程，并支持从任意节点分支重跑对比不同选择的结果。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-trajectory-log]]
%% ytkb:end %%
