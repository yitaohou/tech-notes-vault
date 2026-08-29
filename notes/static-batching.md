---
title: Static Batching
aliases: []
tags:
- concept
summary: static batching 是将固定数量的输入分为一组进行处理的批处理方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Static Batching

%% ytkb:def %%
static batching 是将固定数量的输入分为一组进行处理的批处理方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- static batching 会把固定数量的输入组成一批，但所有请求都必须等到这一批凑满才能处理，实现简单但会导致延迟不稳定。（[66:06](https://youtu.be/JV3pL1_mn2M?t=3966)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dynamic-batching]]
- [[request-batching]]
%% ytkb:end %%
