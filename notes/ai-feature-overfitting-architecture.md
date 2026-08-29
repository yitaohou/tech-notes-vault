---
title: AI Feature Overfitting to Architecture
aliases: []
tags:
- concept
summary: 指用 AI coding agent 逐个实现新功能时，模型为了在单条 prompt 内展示惊艳效果，倾向于把整个架构围绕当前这一个功能重新调整，导致原本稳定的架构被打乱的现象。
created: '2026-08-26'
updated: '2026-08-26'
---

# AI Feature Overfitting to Architecture

%% ytkb:def %%
指用 AI coding agent 逐个实现新功能时，模型为了在单条 prompt 内展示惊艳效果，倾向于把整个架构围绕当前这一个功能重新调整，导致原本稳定的架构被打乱的现象。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-ai-coding-assistants]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:hA_XnzB1Ef8 %%
### 来自 [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof]]
- 用 LLM 编码的第二个问题是：每实现一个新功能，AI 都容易让整个架构向该功能过拟合，因为模型的目标是用单条 prompt 展示尽可能惊艳的效果，却以牺牲此前架构的稳定性为代价。（[00:00](https://youtu.be/hA_XnzB1Ef8?t=0)）
- 好的前端架构不应向任何单一功能过拟合，而应在多个功能需求之间做出折中，形成一个更稳定、更易扩展、也更易解释的公共基础（common ground）。（[00:00](https://youtu.be/hA_XnzB1Ef8?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-prompt-to-ui-overoptimization]]
- [[front-end-system-design]]
%% ytkb:end %%
