---
title: What Should Survive Eval Testing
aliases: []
tags:
- concept
summary: 经过 eval 测试后真正应该留下来的核心内容，包括清楚的目标、必要的 context、可查证的验收方式，以及经反复测试证实确实能修复错误的少数关键规则。
created: '2026-09-03'
updated: '2026-09-03'
---

# What Should Survive Eval Testing

%% ytkb:def %%
经过 eval 测试后真正应该留下来的核心内容，包括清楚的目标、必要的 context、可查证的验收方式，以及经反复测试证实确实能修复错误的少数关键规则。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-evaluation]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Z-4AsgTYv2c %%
### 来自 [[2026-09-02-claude-code-之父建議每六個月刪光你的-claudemd]]
- 经过 eval 测试后真正该留下来的是：清楚的目标、必要的 context、能查证结果的验收方式，以及经过反复测试确实能修复错误的少数关键规则，让每条控制模型行为的规则背后都有明确的测试证据支持，才能用最精简的 prompt 发挥模型最大潜力。（[09:39](https://youtu.be/Z-4AsgTYv2c?t=579)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[prompt-eval-not-permanent-assets]]
- [[pruning-principle]]
%% ytkb:end %%
