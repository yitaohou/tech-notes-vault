---
title: Chunk Size Tradeoff
aliases: []
tags:
- concept
summary: 分片大小选择时需要权衡的取舍：chunk 越小能塞入 context 的信息越多样，但也更容易丢失重要上下文并增加计算开销。
created: '2026-08-26'
updated: '2026-08-26'
---

# Chunk Size Tradeoff

%% ytkb:def %%
分片大小选择时需要权衡的取舍：chunk 越小能塞入 context 的信息越多样，但也更容易丢失重要上下文并增加计算开销。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 更小的 chunk size 能让模型 context 中容纳更多样化的信息片段，但可能丢失重要上下文，且会增加计算开销（尤其是 embedding-based retrieval）。（[33:02](https://youtu.be/JV3pL1_mn2M?t=1982)）
- 不存在普遍适用的最佳 chunk size 或重叠比例，需要针对具体数据和任务反复实验来确定。（[33:02](https://youtu.be/JV3pL1_mn2M?t=1982)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[chunk-overlap]]
- [[text-chunking-rag]]
%% ytkb:end %%
