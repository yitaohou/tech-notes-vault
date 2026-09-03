---
title: Ablation Testing Three-Step Method
aliases: []
tags:
- concept
summary: 对已分类的 instructions 判断哪些可删除时，不需要建大规模测试系统，只需三个简化步骤即可完成的 Ablation 测试流程。
created: '2026-09-03'
updated: '2026-09-03'
---

# Ablation Testing Three-Step Method

%% ytkb:def %%
对已分类的 instructions 判断哪些可删除时，不需要建大规模测试系统，只需三个简化步骤即可完成的 Ablation 测试流程。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-evaluation]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Z-4AsgTYv2c %%
### 来自 [[2026-09-02-claude-code-之父建議每六個月刪光你的-claudemd]]
- Ablation 测试第一步是挑选最常做的任务或最常触发的 Skill，用现有设定跑几次作为对照组，记录文笔、漏填栏位、错误数量与人工调整所花的总时间。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
- Ablation 测试第二步是在乾净 Session 或隔离测试环境中拿掉认为可删除的 Workflow Control（但保留必要 Context 与安全边界），再用完全相同的任务、工具与评分方法重新测试一次。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
- Ablation 测试第三步是观察刪减版本反复出问题的地方，先一次加回一整类规则做初步筛选，若加回后结果确实改善，再拆成单条或小组规则重新细测。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[category-then-individual-rollback-strategy]]
- [[hardcoded-prompt-rules-limitation]]
- [[workflow-control-to-goal-shift]]
%% ytkb:end %%
