---
title: Few-shot Examples Limit Exploration
aliases: []
tags:
- concept
summary: 对于新一代模型，few-shot 示例可能反而限制其探索空间，使其只会照猫画虎、局限于示例展示的用法范围。
created: '2026-08-26'
updated: '2026-08-26'
---

# Few-shot Examples Limit Exploration

%% ytkb:def %%
对于新一代模型，few-shot 示例可能反而限制其探索空间，使其只会照猫画虎、局限于示例展示的用法范围。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-prompt-engineering]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- 对最新模型而言，few-shot 示例可能限制其探索空间，如果给出的例子只展示基础用法，模型可能永远学不会组合使用高级参数。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
- 示例限制模型探索空间的判断仅针对新模型，并非所有模型和工具都不该给示例，老模型仍然需要提供 few-shot 示例。（[03:01](https://youtu.be/Lle_EJljIoo?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[few-shot-prompting-tool-use]]
%% ytkb:end %%
