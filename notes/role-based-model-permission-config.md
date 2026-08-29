---
title: Role-Based Model and Permission Configuration for Sub-Agents
aliases: []
tags:
- concept
summary: 在多Agent循环中，根据子Agent承担的角色差异化配置模型能力、推理强度和权限的设计原则。
created: '2026-08-26'
updated: '2026-08-26'
---

# Role-Based Model and Permission Configuration for Sub-Agents

%% ytkb:def %%
在多Agent循环中，根据子Agent承担的角色差异化配置模型能力、推理强度和权限的设计原则。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 多Agent循环里可以按角色差异化配置：负责安全审查的Agent用能力更强的模型并开启更高推理强度，负责浏览文件的探索型Agent则用速度更快的轻量模型，且只开启只读权限。（[12:04](https://youtu.be/KgiwIEBeOHw?t=724)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-specialization]]
- [[claude-code-agent-teams]]
%% ytkb:end %%
