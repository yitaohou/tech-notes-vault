---
title: Decentralized Multi-Agent Architecture
aliases: []
tags:
- concept
summary: 去中心化（peer-to-peer）多智能体架构指所有 agent 地位平等、没有层级划分，每个 agent 都能与其他任意 agent 通信，依靠外部
  harness 来协调完成任务。
created: '2026-08-26'
updated: '2026-08-26'
---

# Decentralized Multi-Agent Architecture

%% ytkb:def %%
去中心化（peer-to-peer）多智能体架构指所有 agent 地位平等、没有层级划分，每个 agent 都能与其他任意 agent 通信，依靠外部 harness 来协调完成任务。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Mi5wOpAgixw %%
### 来自 [[2026-02-22-multi-agent-systems-explained-in-17-minutes]]
- 去中心化多智能体系统中不存在层级，所有 agent 处于平等地位，各自尝试完成任务，外部围绕它们搭建一层 harness 来协调。（[09:02](https://youtu.be/Mi5wOpAgixw?t=542)）
- 去中心化多智能体架构的优点是设计简单：只需要一组彼此完全相同的 agent 副本，再围绕它们搭建一层 harness 即可运作。（[09:02](https://youtu.be/Mi5wOpAgixw?t=542)）
- 去中心化架构在需要大范围探索的任务（explore-heavy tasks）上表现最佳，在相关 benchmark 中是同类架构里的最佳表现者。（[09:02](https://youtu.be/Mi5wOpAgixw?t=542)）
- 去中心化架构的缺点是协调成本最大化：由于每个 agent 都能与所有其他 agent 通信、且没有明确的主导者，一个 agent 的发现要传播给所有其他 agent 就必须逐一通信或依赖共享上下文，这会让 harness 的构建变得复杂且需针对具体任务定制。（[09:02](https://youtu.be/Mi5wOpAgixw?t=542)）
- 去中心化（decentralized）架构就像一群 agent（swarm）共同围攻同一个问题，没有统一的领导者进行调度。（[15:06](https://youtu.be/Mi5wOpAgixw?t=906)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-harness]]
- [[centralized-multi-agent-architecture]]
- [[hybrid-multi-agent-architecture]]
%% ytkb:end %%
