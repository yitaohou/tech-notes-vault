---
title: LLM-as-a-Judge
aliases: []
tags:
- concept
summary: 使用另一个 AI 模型作为评判者，来评估生产环境中 AI 模型输出质量的方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# LLM-as-a-Judge

%% ytkb:def %%
使用另一个 AI 模型作为评判者，来评估生产环境中 AI 模型输出质量的方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-evaluation]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- LLM-as-a-judge 相比人类评估者速度更快、更易用、成本更低，且不需要参考数据即可评判 correctness、toxicity、hallucination 等属性。（[12:01](https://youtu.be/JV3pL1_mn2M?t=721)）
- 研究表明 AI judge 与人类评估者的相关性可以很强，其与人类评分的一致性有时甚至高于不同人类评审员之间的一致性。（[12:01](https://youtu.be/JV3pL1_mn2M?t=721)）
- AI judge 除了给出评分，还能解释其判断依据，这有助于提升评估过程的透明度。（[12:01](https://youtu.be/JV3pL1_mn2M?t=721)）
- AI judge 有三种典型使用方式：对输出打分、将输出与参考答案比较、或在两个回答中选出更优的一个。（[12:01](https://youtu.be/JV3pL1_mn2M?t=721)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-judge-bias]]
- [[ai-judge-classification-vs-scoring]]
- [[ai-judge-limitations]]
- [[ai-judge-prompt-design]]
%% ytkb:end %%
