---
title: Pruning（修剪原则）
aliases: []
tags:
- concept
summary: writing-great-skills 提出的第一个原则：删除提示词里所有废话、会让 AI 分心的文字，以及模型本来就知道该怎么做的指令。
created: '2026-08-26'
updated: '2026-09-03'
---

# Pruning（修剪原则）

%% ytkb:def %%
writing-great-skills 提出的第一个原则：删除提示词里所有废话、会让 AI 分心的文字，以及模型本来就知道该怎么做的指令。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:aR97E7aKEgg %%
### 来自 [[2026-07-22-700-萬人下載的-grill-mematt-pocock-到底寫了什麼]]
- Pruning 原则的核心理念是，在 AI 面前多写一句废话，AI 就多一分分心的可能，因此要修剪掉所有非必要文字，哪怕是模型自己也知道该怎么做的指令。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
%% ytkb:end %%

%% ytkb:video:Z-4AsgTYv2c %%
### 来自 [[2026-09-02-claude-code-之父建議每六個月刪光你的-claudemd]]
- 判断提示词中某条规则是否该保留的自检问题之一：这句话有没有真的改变模型的行为，如果模型本来就会这样做，这句话就只是在吃掉 context，可以直接删掉。（[12:47](https://youtu.be/Z-4AsgTYv2c?t=767)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[avoid-redundant-instructions]]
- [[claude-md-file]]
- [[context-dilution]]
- [[matt-pocock]]
- [[writing-great-skills-skill]]
%% ytkb:end %%
