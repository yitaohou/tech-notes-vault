---
title: Coding Agent Harness Convergence
aliases: []
tags:
- concept
summary: 指 Claude Code、Codex、Cursor 等主流编码 agent 的核心接口和通用工作循环已趋于一致的现象。
created: '2026-08-26'
updated: '2026-08-26'
---

# Coding Agent Harness Convergence

%% ytkb:def %%
指 Claude Code、Codex、Cursor 等主流编码 agent 的核心接口和通用工作循环已趋于一致的现象。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- 主流编码agent的通用循环是：先观察整个代码仓库、做规划，接着搜索和读取相关文件，再编辑或打补丁写测试，然后运行检查错误，循环往复直到任务完成，就像人类开发者用 IDE 工作一样。（[03:03](https://youtu.be/z_F0z7wF5XU?t=183)）
%% ytkb:end %%

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- Claude Code 与 Codex 都各自实现了功能几乎相同的/goal 能力，体现出整个编码Agent行业发展方向的高度一致性。（[06:03](https://youtu.be/KgiwIEBeOHw?t=363)）
- 有人总结的循环组成清单与 Codex、Claude Code 的产品功能几乎一一对应，说明不同 Coding Agent 工具的底层架构已趋于一致，因此不必纠结选哪款工具，只需设计一套通用循环逻辑即可跨工具运行。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-code]]
- [[codex]]
- [[coding-agent]]
- [[goal-directed-persistent-loop]]
- [[loop-engineering]]
%% ytkb:end %%
