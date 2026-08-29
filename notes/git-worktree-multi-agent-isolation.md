---
title: Git Worktree for Multi-Agent File Isolation
aliases: []
tags:
- concept
summary: 利用 Git 的工作树（worktree）功能为每个并行运行的 Agent 创建独立工作目录与分支，从物理层面避免多 Agent 同时修改同一文件导致的冲突。
created: '2026-08-26'
updated: '2026-08-26'
---

# Git Worktree for Multi-Agent File Isolation

%% ytkb:def %%
利用 Git 的工作树（worktree）功能为每个并行运行的 Agent 创建独立工作目录与分支，从物理层面避免多 Agent 同时修改同一文件导致的冲突。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 工作树（Worktrees）模块用于解决多Agent并行运行时的文件冲突问题：同时运行多个Agent很容易出现多个Agent修改同一文件、最终代码冲突导致任务失败的情况。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- Git 的工作树功能可以创建一个独立工作目录并运行在单独分支上，但共享同一代码仓库的历史记录，使一个Agent的修改从物理层面碰不到另一个Agent的工作目录，从根源上避免文件冲突。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- Codex 把工作树支持直接内置到产品里，多个执行线程可以同时访问同一代码仓库而互相之间不会产生干扰。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- Claude Code 支持原生Git工作树功能，可以通过 --worktree 参数在独立代码副本里开启会话，也可以给子Agent设置工作树隔离配置，任务结束后自动清理工作目录。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
%% ytkb:end %%
