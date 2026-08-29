---
title: Perplexity
aliases: []
tags:
- concept
summary: Perplexity（困惑度）是 cross entropy 的指数值，衡量模型预测下一个 token 时的不确定性程度。
created: '2026-08-26'
updated: '2026-08-26'
---

# Perplexity

%% ytkb:def %%
Perplexity（困惑度）是 cross entropy 的指数值，衡量模型预测下一个 token 时的不确定性程度。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-llm-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- Perplexity 是 cross entropy 的指数值，衡量模型预测下一个 token 时的不确定性，perplexity 越高说明模型认为可能的候选选项越多。（[09:01](https://youtu.be/JV3pL1_mn2M?t=541)）
- 怎样的 perplexity 算好完全取决于数据本身：结构性越强的数据可预测性越高，预期的 perplexity 也越低。（[09:01](https://youtu.be/JV3pL1_mn2M?t=541)）
- 词表（vocabulary）越大，perplexity 通常越高，因为模型需要考虑的可能选项更多。（[09:01](https://youtu.be/JV3pL1_mn2M?t=541)）
- 上下文长度越长，perplexity 往往越低。（[09:01](https://youtu.be/JV3pL1_mn2M?t=541)）
- 对于经过 SFT 或 RLHF 等大幅度 post-training 的模型，perplexity 的可靠性会下降：模型在完成实际任务方面变得更好，但从统计角度预测下一个 token 的能力可能反而变差。（[09:01](https://youtu.be/JV3pL1_mn2M?t=541)）
- Perplexity 可用于检测某段文本是否出现在模型的训练数据中，因为模型对训练数据中的内容通常能异常准确地预测。（[09:01](https://youtu.be/JV3pL1_mn2M?t=541)）
- Perplexity 也可用于识别无意义文本（nonsensical text），这类文本通常会表现出异常高的 perplexity。（[09:01](https://youtu.be/JV3pL1_mn2M?t=541)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cross-entropy]]
%% ytkb:end %%
