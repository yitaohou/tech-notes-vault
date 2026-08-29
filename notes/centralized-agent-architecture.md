---
title: Centralized Multi-Agent Architecture
aliases: []
tags:
- concept
summary: 多智能体系统中由一个lead agent（orchestrator）负责协调并将任务委派给多个worker sub-agent的架构模式，与自由协作的swarm相对。
created: '2026-08-26'
updated: '2026-08-26'
---

# Centralized Multi-Agent Architecture

%% ytkb:def %%
多智能体系统中由一个lead agent（orchestrator）负责协调并将任务委派给多个worker sub-agent的架构模式，与自由协作的swarm相对。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Mi5wOpAgixw %%
### 来自 [[2026-02-22-multi-agent-systems-explained-in-17-minutes]]
- 在centralized architecture中，一个lead agent（orchestrator）负责将任务委派给一组worker agent，而不是让多个agent以swarm形式自由协作攻克问题。（[12:04](https://youtu.be/Mi5wOpAgixw?t=724)）
- centralized architecture中若某个sub-agent出错，该错误只会传回lead agent由其核实校正，而不会立即扩散到其他sub-agent，这是其错误放大程度低的原因。（[12:04](https://youtu.be/Mi5wOpAgixw?t=724)）
- centralized architecture的缺点是系统复杂度较高，且设计其协调框架（harness）本身是一项非平凡（nontrivial）的工作。（[12:04](https://youtu.be/Mi5wOpAgixw?t=724)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[anthropic-multi-agent-research-system]]
- [[decentralized-swarm-architecture]]
- [[error-amplification-multi-agent]]
- [[hybrid-agent-architecture]]
%% ytkb:end %%
