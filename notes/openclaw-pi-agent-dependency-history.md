---
title: OpenClaw's Historical Dependency on Pi Agent
aliases: []
tags:
- concept
summary: OpenClaw 项目在早期版本（如 2026 年 2 月，其大火期间）曾依赖 pi-coding-agent、pi-agent-core、pi-ai、pi-tui
  等 Pi Agent 相关包作为底层架构，后续版本中这些依赖已被移除。
created: '2026-09-03'
updated: '2026-09-03'
---

# OpenClaw's Historical Dependency on Pi Agent

%% ytkb:def %%
OpenClaw 项目在早期版本（如 2026 年 2 月，其大火期间）曾依赖 pi-coding-agent、pi-agent-core、pi-ai、pi-tui 等 Pi Agent 相关包作为底层架构，后续版本中这些依赖已被移除。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:j0Z5cngKDeo %%
### 来自 [[2026-07-27-我为什么对-pi-agent-产生了兴趣]]
- 作者在 Pi Agent 官网看到「See OpenClaw for a real-world example」的说明，但在 OpenClaw 当前代码仓库的 package.json 及全局搜索中都找不到 Pi Agent 的痕迹。（[00:00](https://youtu.be/j0Z5cngKDeo?t=0)）
- 作者将 OpenClaw 代码仓库切换到 2026 年 2 月的早期分支后进行搜索，确认当时确实依赖了 pi-coding-agent、pi-agent-core、pi-ai、pi-tui 等多个 Pi Agent 相关项目，说明 OpenClaw 早期把 Pi Agent 的能力直接嵌入了自身产品，只是后续架构逐渐演变后不再使用。（[00:00](https://youtu.be/j0Z5cngKDeo?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[pi-agent]]
%% ytkb:end %%
