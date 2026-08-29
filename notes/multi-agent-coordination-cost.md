---
title: Multi-Agent Coordination Cost
aliases: []
tags:
- concept
summary: 将系统从单代理扩展为多代理时，代理之间需要协作，这会产生额外的计算开销，即协调成本。
created: '2026-08-26'
updated: '2026-08-26'
---

# Multi-Agent Coordination Cost

%% ytkb:def %%
将系统从单代理扩展为多代理时，代理之间需要协作，这会产生额外的计算开销，即协调成本。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Mi5wOpAgixw %%
### 来自 [[2026-02-22-multi-agent-systems-explained-in-17-minutes]]
- 把系统从单代理扩展到多代理会引入代理间协作的协调任务，带来额外的计算成本。（[04:40](https://youtu.be/Mi5wOpAgixw?t=280)）
%% ytkb:end %%

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 子Agent会消耗更多token，因为每个Agent都要独立完成模型调用和工具使用，所以子Agent机制不需要到处使用，只在需要二次把关的关键场景开启才划算。（[13:00](https://youtu.be/KgiwIEBeOHw?t=780)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[explorer-implementer-verifier-agent-pattern]]
- [[google-research-45-percent-threshold]]
%% ytkb:end %%
