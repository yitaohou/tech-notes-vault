---
title: PEFT Inference Latency Tradeoff
aliases: []
tags:
- concept
summary: PEFT 技术虽能减少训练所需的可训练参数，但可能因插入额外参数而增加推理延迟。
created: '2026-08-26'
updated: '2026-08-26'
---

# PEFT Inference Latency Tradeoff

%% ytkb:def %%
PEFT 技术虽能减少训练所需的可训练参数，但可能因插入额外参数而增加推理延迟。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- PEFT 技术通过在模型策略性位置插入额外参数来实现高效微调，但这种做法可能会增加 inference latency。（[45:04](https://youtu.be/JV3pL1_mn2M?t=2704)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[parameter-efficient-fine-tuning]]
%% ytkb:end %%
