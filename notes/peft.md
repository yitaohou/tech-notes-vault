---
title: PEFT (Parameter-Efficient Fine-Tuning)
aliases: []
tags:
- concept
summary: 只更新模型少量参数（如通过 adapter）即可完成微调的高效方法，代表技术包括 LoRA。
created: '2026-08-26'
updated: '2026-08-26'
---

# PEFT (Parameter-Efficient Fine-Tuning)

%% ytkb:def %%
只更新模型少量参数（如通过 adapter）即可完成微调的高效方法，代表技术包括 LoRA。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- PEFT 方法在数百条样本量级即可产生效果，远少于 full fine-tuning 所需的数据量。（[51:04](https://youtu.be/JV3pL1_mn2M?t=3064)）
- 数据量有限（几百到几千条）时，使用 PEFT 方法通常比全参数微调（full fine-tuning）效果更好。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[full-fine-tuning]]
- [[lora]]
- [[lora-adapter-fine-tuning]]
%% ytkb:end %%
