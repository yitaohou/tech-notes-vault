---
title: Generator-Verifier Agent Separation
aliases: []
tags:
- concept
summary: 在自动化循环中把负责生成代码的 Agent 和负责验证的子 Agent 分开设置，用以提升循环给出「完成」结论可信度的设计方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Generator-Verifier Agent Separation

%% ytkb:def %%
在自动化循环中把负责生成代码的 Agent 和负责验证的子 Agent 分开设置，用以提升循环给出「完成」结论可信度的设计方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- 把生成代码的 Agent 和验证的子 Agent 分开，是为了让循环给出的完成结论更有参考性，但「完成」本身仍只是一个声明，而不是经过严格验证的结论。（[15:04](https://youtu.be/KgiwIEBeOHw?t=904)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-specialization]]
- [[unattended-loop-verification-responsibility]]
%% ytkb:end %%
