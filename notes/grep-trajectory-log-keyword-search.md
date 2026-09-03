---
title: Grep Trajectory Log Keyword Search
aliases: []
tags:
- concept
summary: 应急响应第二步，用grep命令在轨迹日志中搜索敏感调用关键词，判断是否发生了完整攻击链。
created: '2026-09-03'
updated: '2026-09-03'
---

# Grep Trajectory Log Keyword Search

%% ytkb:def %%
应急响应第二步，用grep命令在轨迹日志中搜索敏感调用关键词，判断是否发生了完整攻击链。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 用grep搜索轨迹日志里的关键词（如插件定义接口、插件运行接口和subprocess）三个敏感调用，一旦命中说明很可能有人在机器里走通了从注入到执行的完整攻击链。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[grep-periodic-monitoring]]
- [[incident-response-timeline-localization]]
%% ytkb:end %%
