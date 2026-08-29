---
title: Selective Caching Policy for Frontend Bundles
aliases: []
tags:
- concept
summary: 根据前端不同代码块变化频率的差异，分别设置不同缓存策略（而非对整个 bundle 用同一策略）的做法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Selective Caching Policy for Frontend Bundles

%% ytkb:def %%
根据前端不同代码块变化频率的差异，分别设置不同缓存策略（而非对整个 bundle 用同一策略）的做法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-performance-optimization]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 前端应用中变化很少的部分（如设计系统、核心逻辑、稳定的第三方库）应该和经常变化的部分分开打包，从而可以对它们分别设置不同的缓存策略。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[app-logic-chunk-short-max-age]]
- [[frontend-bundle-splitting]]
- [[stable-vendor-chunk-long-max-age]]
%% ytkb:end %%
