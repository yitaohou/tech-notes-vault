---
title: Decoupled Prefill and Decode
aliases: []
tags:
- concept
summary: decoupled prefill and decode 指将 LLM 推理中计算特性不同的 prefill 阶段与 decode 阶段分开处理的优化技术。
created: '2026-08-26'
updated: '2026-08-26'
---

# Decoupled Prefill and Decode

%% ytkb:def %%
decoupled prefill and decode 指将 LLM 推理中计算特性不同的 prefill 阶段与 decode 阶段分开处理的优化技术。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 由于 prefill 和 decode 两个阶段的计算需求不同，将它们解耦分开处理可以避免资源争抢、提升整体效率。（[66:06](https://youtu.be/JV3pL1_mn2M?t=3966)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[request-batching]]
%% ytkb:end %%
