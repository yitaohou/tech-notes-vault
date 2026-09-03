---
title: Single-Epoch Training for Hallucination Prevention
aliases: []
tags:
- concept
summary: 在临床模型微调中刻意只进行一个训练周期（epoch），以避免模型因过度训练而产生幻觉的做法。
created: '2026-09-02'
updated: '2026-09-02'
---

# Single-Epoch Training for Hallucination Prevention

%% ytkb:def %%
在临床模型微调中刻意只进行一个训练周期（epoch），以避免模型因过度训练而产生幻觉的做法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:HdkhI6VyQD0 %%
### 来自 [[2026-09-01-臨床小型語言模型的運作原理]]
- 该蒸馏流程刻意只在本地端进行单一周期的训练，因为训练次数过多会让模型容易产生幻觉、胡说八道，这在医疗场景中是绝对禁忌。（[03:00](https://youtu.be/HdkhI6VyQD0?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[hallucination]]
- [[lora]]
%% ytkb:end %%
