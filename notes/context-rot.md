---
title: Context Rot
aliases: []
tags:
- concept
summary: 指即便上下文窗口容量很大（如百万 token 级别），随着窗口被填入的 token 越来越多，模型表现反而趋于下降的现象。
created: '2026-08-26'
updated: '2026-08-26'
---

# Context Rot

%% ytkb:def %%
指即便上下文窗口容量很大（如百万 token 级别），随着窗口被填入的 token 越来越多，模型表现反而趋于下降的现象。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Mi5wOpAgixw %%
### 来自 [[2026-02-22-multi-agent-systems-explained-in-17-minutes]]
- context rot 现象表明，即使拥有百万 token 级别的大上下文窗口，随着窗口填充度增加，模型表现依然会明显下降。（[00:00](https://youtu.be/Mi5wOpAgixw?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[chromadb-context-rot-study]]
- [[test-time-compute-scaling]]
%% ytkb:end %%
