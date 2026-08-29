---
title: Lexical Similarity Evaluation
aliases: []
tags:
- concept
summary: 衡量输出文本与参考文本之间 token 重叠程度的连续型评估指标。
created: '2026-08-26'
updated: '2026-08-26'
---

# Lexical Similarity Evaluation

%% ytkb:def %%
衡量输出文本与参考文本之间 token 重叠程度的连续型评估指标。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-evaluation]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- lexical similarity 的常见实现技术包括 edit distance（将一段文本转换为另一段所需的最少改动次数）和 n-gram overlap 指标（如 BLEU、Rouge）。（[12:01](https://youtu.be/JV3pL1_mn2M?t=721)）
- lexical similarity 的缺点是需要一套全面的参考答案集合，参考答案本身也可能有误，且更高的 lexical similarity 不代表回答质量更好，因为同一意思可以用多种方式表达。（[12:01](https://youtu.be/JV3pL1_mn2M?t=721)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[reference-based-evaluation]]
%% ytkb:end %%
