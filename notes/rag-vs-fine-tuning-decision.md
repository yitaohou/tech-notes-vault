---
title: RAG vs Fine-tuning Decision
aliases: []
tags:
- concept
summary: 指根据模型失败的原因是信息不足还是行为问题来决定选择 RAG 还是 fine-tuning 的判断标准。
created: '2026-08-26'
updated: '2026-08-26'
---

# RAG vs Fine-tuning Decision

%% ytkb:def %%
指根据模型失败的原因是信息不足还是行为问题来决定选择 RAG 还是 fine-tuning 的判断标准。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 在 prompting 已经榨干效果之后，若模型失败是因为缺乏信息（如私有公司数据或近期事件），RAG 能让模型获取这些信息；若模型失败是行为层面的问题（如答案内容正确但不相关或格式不对），fine-tuning 可能更有帮助；如果两种问题都存在，就应该两者结合。（[42:04](https://youtu.be/JV3pL1_mn2M?t=2524)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[fine-tuning]]
- [[retrieval-augmented-generation]]
%% ytkb:end %%
