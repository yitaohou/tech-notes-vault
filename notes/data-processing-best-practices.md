---
title: Data Processing Best Practices
aliases: []
tags:
- concept
summary: 拿到训练数据后为保证质量而执行的一系列处理步骤，包括过滤、去重、清洗、格式化等。
created: '2026-08-26'
updated: '2026-08-26'
---

# Data Processing Best Practices

%% ytkb:def %%
拿到训练数据后为保证质量而执行的一系列处理步骤，包括过滤、去重、清洗、格式化等。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-training-data]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 在大规模处理数据前，应先用小规模的过滤任务和测试脚本进行验证，并避免直接在原始数据上修改、需保留数据原件。（[57:04](https://youtu.be/JV3pL1_mn2M?t=3424)）
- 数据处理中应对分布和异常值做探索性数据分析（EDA），并检查标注者之间的不一致（interannotator disagreement）以解决冲突。（[57:04](https://youtu.be/JV3pL1_mn2M?t=3424)）
- 数据处理应包含事实核查与人工抽查样本、对数据去重以防止某些样本被过度重复代表。（[57:04](https://youtu.be/JV3pL1_mn2M?t=3424)）
- 清理HTML、markdown等格式标记类token可以提升模型表现，同时减少输入长度。（[57:04](https://youtu.be/JV3pL1_mn2M?t=3424)）
- 数据处理应移除包含PII、有毒内容或受版权保护内容等不合规数据，并过滤掉质量核验中识别出的低质量数据。（[57:04](https://youtu.be/JV3pL1_mn2M?t=3424)）
- 还需确保数据以正确格式提供给目标模型，即使用与该模型匹配的tokenizer和chat template。（[57:04](https://youtu.be/JV3pL1_mn2M?t=3424)）
- 精心处理好的数据集质量往往是模型表现从平庸走向卓越的关键区别所在。（[57:04](https://youtu.be/JV3pL1_mn2M?t=3424)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[active-learning]]
%% ytkb:end %%
