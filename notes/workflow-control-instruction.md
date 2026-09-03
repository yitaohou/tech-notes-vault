---
title: Workflow Control Instruction Category
aliases: []
tags:
- concept
summary: instructions 三分类中的第二类，指规定模型必须遵循的流程细节（如固定格式、工具调用顺序），常是为弥补旧模型能力不足而留下的补丁，是最值得优先测试是否可删的一类。
created: '2026-09-03'
updated: '2026-09-03'
---

# Workflow Control Instruction Category

%% ytkb:def %%
instructions 三分类中的第二类，指规定模型必须遵循的流程细节（如固定格式、工具调用顺序），常是为弥补旧模型能力不足而留下的补丁，是最值得优先测试是否可删的一类。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Z-4AsgTYv2c %%
### 来自 [[2026-09-02-claude-code-之父建議每六個月刪光你的-claudemd]]
- Workflow Control 类规则（如强制每段列三点、工具必须按固定顺序使用、把模型本来就会的动作写死）最可能是为旧模型留下的补丁，因此是最值得优先做消融测试的一类。（[03:01](https://youtu.be/Z-4AsgTYv2c?t=181)）
- 即使是与品质相关的 workflow control 规则，也可能因模型能力提升而不再需要出现，这类规则应通过消融测试来判断是否可以拿掉，而非直接假设无用。（[03:01](https://youtu.be/Z-4AsgTYv2c?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ablation-study-prompt-testing]]
- [[hard-coded-prompt-rules]]
- [[hardcoded-prompt-rules-limitation]]
- [[instruction-three-category-framework]]
%% ytkb:end %%
