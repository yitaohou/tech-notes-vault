---
title: Harness Engineering
aliases: []
tags:
- concept
summary: 围绕基础模型搭建的整套支撑系统进行设计与优化的工程实践，负责编排执行流程、规划、工具调用、上下文管理、结果评估等。
created: '2026-08-26'
updated: '2026-08-26'
---

# Harness Engineering

%% ytkb:def %%
围绕基础模型搭建的整套支撑系统进行设计与优化的工程实践，负责编排执行流程、规划、工具调用、上下文管理、结果评估等。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- Lilian Weng 认为，连接原始模型与真实应用场景之间的部署系统（harness），其重要性可能不亚于模型本身的原生智能。（[00:00](https://youtu.be/z_F0z7wF5XU?t=0)）
- Harness 是包裹在基础模型外面的整套系统，负责编排执行流程，决定模型如何思考规划、如何调用工具行动、如何感知和管理上下文、如何存储产物以及如何评估结果。（[00:00](https://youtu.be/z_F0z7wF5XU?t=0)）
- Claude Code、Codex 这类成功的编码 Agent 产品，其核心竞争力很大程度上来自成熟的 Harness 设计。（[00:00](https://youtu.be/z_F0z7wF5XU?t=0)）
- Harness 的设计原则是尽量简单通用以保证泛化性，这一思路大量借鉴了现有软件工程实践，也能复用模型预训练中学到的相关知识。（[00:00](https://youtu.be/z_F0z7wF5XU?t=0)）
- Harness 的定位与操作系统类似，把复杂逻辑封装在系统内部、对外保持简洁接口；未来行业里的配置和工具接口协议大概率也会逐步走向标准化。（[00:00](https://youtu.be/z_F0z7wF5XU?t=0)）
%% ytkb:end %%

%% ytkb:video:KgiwIEBeOHw %%
### 来自 [[2026-06-16-什么是循环工程loop-engineering-coding-agent-子agent-mcp协议]]
- Agent Harness Engineering 指为单个 Agent 搭建运行环境框架的工程实践，位于循环工程之下的一层。（[03:01](https://youtu.be/KgiwIEBeOHw?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-definition]]
- [[claude-code]]
- [[deep-module]]
- [[loop-engineering]]
- [[recursive-self-improvement]]
%% ytkb:end %%
