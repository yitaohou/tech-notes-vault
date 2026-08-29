---
title: Training Data Quality Factors
aliases: []
tags:
- concept
summary: 衡量微调训练数据是否为「高质量」的一组考量维度，包括 relevance、alignment、consistency、formatting、uniqueness、compliance、coverage
  等。
created: '2026-08-26'
updated: '2026-08-26'
---

# Training Data Quality Factors

%% ytkb:def %%
衡量微调训练数据是否为「高质量」的一组考量维度，包括 relevance、alignment、consistency、formatting、uniqueness、compliance、coverage 等。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-training-data]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 训练数据的 relevance 指示例应与目标任务相关，例如 19 世纪的法律文本对回答当代法律问题可能没有帮助。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
- 训练数据需要与任务要求对齐（alignment）：若任务注重 factual consistency，标注需事实正确；若任务需要创造性，标注也应体现创造性。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
- 训练数据的 consistency 指标注在不同示例和不同标注者之间应保持一致。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
- 训练数据应正确格式化（correctly formatted），即符合预期的结构规范。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
- 训练数据需要具备足够的独特性（uniqueness），即数据集中应尽量减少重复样本。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
- 训练数据需要合规（compliant），遵循内部和外部的相关政策。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
- 训练数据需要具备覆盖度（coverage），即涵盖目标任务的所有可能问题类型；某个重要领域覆盖不足，无论数据总量多大，该领域的表现都会很差。（[54:04](https://youtu.be/JV3pL1_mn2M?t=3244)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[llama-3-human-data-quality-issue]]
%% ytkb:end %%
