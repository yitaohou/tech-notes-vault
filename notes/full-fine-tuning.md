---
title: Full Fine-tuning
aliases: []
tags:
- concept
summary: 全量微调（full fine-tuning）指更新模型全部参数的微调方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Full Fine-tuning

%% ytkb:def %%
全量微调（full fine-tuning）指更新模型全部参数的微调方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- full fine-tuning（更新全部模型参数）在早期小模型时代很常见，但需要大量高质量标注数据和大量计算资源。（[45:04](https://youtu.be/JV3pL1_mn2M?t=2704)）
- full fine-tuning 通常需要数千到数百万条训练样本才能取得良好效果。（[51:04](https://youtu.be/JV3pL1_mn2M?t=3064)）
- full fine-tuning 通常需要几万到几百万条样本量级的数据；而只有几百到几千条样本时，PEFT 方法（如 LoRA）效果通常更好。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[lora]]
- [[lora-adapter-fine-tuning]]
- [[parameter-efficient-fine-tuning]]
- [[partial-fine-tuning]]
- [[peft]]
%% ytkb:end %%
