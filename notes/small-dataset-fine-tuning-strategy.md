---
title: Small Dataset Fine-Tuning Strategy
aliases: []
tags:
- concept
summary: 在投入构建大数据集之前，先用少量精心制作的样本（约 50 条）测试微调是否有效的实践策略。
created: '2026-08-26'
updated: '2026-08-26'
---

# Small Dataset Fine-Tuning Strategy

%% ytkb:def %%
在投入构建大数据集之前，先用少量精心制作的样本（约 50 条）测试微调是否有效的实践策略。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 建议先用约 50 条精心制作的样本做微调测试：如果效果有明显提升，加更多数据大概率会进一步帮助；如果没有提升，加大数据集通常解决不了问题，除非先排除超参数或数据质量等其他问题。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
- 在大多数情况下，用 50 到 100 条样本做微调后就应该能看到明显的效果提升。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[progressive-fine-tuning-strategy]]
%% ytkb:end %%
