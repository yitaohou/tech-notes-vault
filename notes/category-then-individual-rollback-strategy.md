---
title: Category-then-individual Rollback Strategy
aliases: []
tags:
- concept
summary: 排查该恢复哪些被删除规则时，先整类加回测试确认有效、再拆分成单条规则细测的排查方法。
created: '2026-09-03'
updated: '2026-09-03'
---

# Category-then-individual Rollback Strategy

%% ytkb:def %%
排查该恢复哪些被删除规则时，先整类加回测试确认有效、再拆分成单条规则细测的排查方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-evaluation]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Z-4AsgTYv2c %%
### 来自 [[2026-09-02-claude-code-之父建議每六個月刪光你的-claudemd]]
- 如果拿掉某条规则后测试结果不但没有变差、甚至还变得更好，那这条规则就可以准备正式删除。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ablation-testing-three-step-method]]
- [[multi-run-average-comparison]]
%% ytkb:end %%
