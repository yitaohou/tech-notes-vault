---
title: Multi-run Average Comparison
aliases: []
tags:
- concept
summary: 由于模型输出具有随机性，需要让新旧设定针对同一组任务各自多跑几次，再比较多次测试的平均表现而非单次最佳结果。
created: '2026-09-03'
updated: '2026-09-03'
---

# Multi-run Average Comparison

%% ytkb:def %%
由于模型输出具有随机性，需要让新旧设定针对同一组任务各自多跑几次，再比较多次测试的平均表现而非单次最佳结果。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-evaluation]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Z-4AsgTYv2c %%
### 来自 [[2026-09-02-claude-code-之父建議每六個月刪光你的-claudemd]]
- 因为模型输出带有随机性，同一组任务在新旧设定下都必须各跑几次，比较的是这两个版本在多次测试中的平均表现、失败率与稳定度，而不是各挑一次最好的结果来比。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ablation-testing-three-step-method]]
%% ytkb:end %%
