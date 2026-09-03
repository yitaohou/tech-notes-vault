---
title: Periodic Grep Monitoring as Alarm
aliases: []
tags:
- concept
summary: 定期运行grep搜索轨迹日志敏感关键词的命令，将其当作简易报警器使用的做法。
created: '2026-09-03'
updated: '2026-09-03'
---

# Periodic Grep Monitoring as Alarm

%% ytkb:def %%
定期运行grep搜索轨迹日志敏感关键词的命令，将其当作简易报警器使用的做法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 这条grep敏感关键词的命令平时也可以当报警器用，隔一阵子跑一遍，一旦发现命中就说明有攻击事件发生。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[grep-trajectory-log-keyword-search]]
- [[inotifywait-log-monitoring]]
%% ytkb:end %%
