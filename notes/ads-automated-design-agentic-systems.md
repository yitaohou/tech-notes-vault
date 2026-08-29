---
title: Automated Design of Agentic Systems (ADAS)
aliases: []
tags:
- concept
summary: 把 agent 设计本身形式化为优化问题，通过「元 agent 搜索」自动发现新 agent 工作流的方法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Automated Design of Agentic Systems (ADAS)

%% ytkb:def %%
把 agent 设计本身形式化为优化问题，通过「元 agent 搜索」自动发现新 agent 工作流的方法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- ADAS 先在存档里初始化思维链、自我优化等简单 agent 方案，再让元 agent 参考存档中的现有方案编写新的 agent 代码：先写高层工作流描述，再实现为可执行代码，并经两轮自我优化检查新颖性与正确性，评估合格的新 agent 即加回存档，如此反复迭代。（[12:08](https://youtu.be/z_F0z7wF5XU?t=728)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[aflow-agentic-workflow-search]]
- [[agentic-workflow-design-as-search-problem]]
%% ytkb:end %%
