---
title: Prompt Lookup Decoding (Inference with Reference)
aliases: []
tags:
- concept
summary: Inference with reference（prompt lookup decoding）是一种在合适场景下直接从输入中复制 token、而非从头生成的推理加速技术。
created: '2026-08-26'
updated: '2026-08-26'
---

# Prompt Lookup Decoding (Inference with Reference)

%% ytkb:def %%
Inference with reference（prompt lookup decoding）是一种在合适场景下直接从输入中复制 token、而非从头生成的推理加速技术。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-inference-optimization]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 在回答关于某篇文档的问题等场景下，直接从输入内容中复制 token 而非重新生成，可以显著加快基于文档查询的响应速度。（[63:05](https://youtu.be/JV3pL1_mn2M?t=3785)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[autoregressive-generation-bottleneck]]
%% ytkb:end %%
