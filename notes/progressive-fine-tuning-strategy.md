---
title: Progressive Fine-Tuning Strategy
aliases: []
tags:
- concept
summary: 通过先在更易获得的数据上微调、再逐步过渡到目标高质量数据的分阶段策略，用于降低对稀缺目标数据的依赖量。
created: '2026-08-26'
updated: '2026-08-26'
---

# Progressive Fine-Tuning Strategy

%% ytkb:def %%
通过先在更易获得的数据上微调、再逐步过渡到目标高质量数据的分阶段策略，用于降低对稀缺目标数据的依赖量。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 一种 curriculum 策略是先做 self-supervised 微调（在领域文档上训练），再做 supervised 微调（在目标问答对上训练）。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
- 另一种 curriculum 策略是先在数据丰富的相邻领域（adjacent domain）上微调，再迁移到数据稀缺的目标领域上继续微调。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
- 第三种 curriculum 策略是先在 AI 生成的 synthetic 数据上微调，再用有限的真实数据（real data）继续微调。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[small-dataset-fine-tuning-strategy]]
%% ytkb:end %%
