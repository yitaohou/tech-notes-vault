---
title: Goal-Directed Persistent Loop (/goal)
aliases: []
tags:
- concept
summary: 与按固定节奏重复运行的/loop不同，/goal 指令会持续运行直到用户设定的可验证条件真正达成才停止。
created: '2026-08-26'
updated: '2026-08-26'
---

# Goal-Directed Persistent Loop (/goal)

%% ytkb:def %%
与按固定节奏重复运行的/loop不同，/goal 指令会持续运行直到用户设定的可验证条件真正达成才停止。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- /goal 指令不同于按固定节奏重复运行的/loop，它会持续运行，直到用户设定的条件真正达成为止，无需人工盯着进程。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- /goal 的停止条件用自然语言描述可验证标准即可，例如「保证认证模块的所有测试全部通过，并且代码格式检查没有问题」，满足后循环自动结束。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- Codex 也提供了同名的/goal 功能，可以跨多轮对话持续工作直到可验证的停止条件成立，并支持暂停、恢复和清除任务。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[coding-agent-harness-convergence]]
- [[goal-verifier-separate-agent]]
%% ytkb:end %%
