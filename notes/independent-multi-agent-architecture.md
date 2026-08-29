---
title: Independent Multi-Agent Architecture
aliases: []
tags:
- concept
summary: 四大 multi-agent 架构之一，指并行运行多个互不通信的独立 agent 实例，各自独立完成同一任务后再汇总结果。
created: '2026-08-26'
updated: '2026-08-26'
---

# Independent Multi-Agent Architecture

%% ytkb:def %%
四大 multi-agent 架构之一，指并行运行多个互不通信的独立 agent 实例，各自独立完成同一任务后再汇总结果。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Mi5wOpAgixw %%
### 来自 [[2026-02-22-multi-agent-systems-explained-in-17-minutes]]
- 独立式（independent）multi-agent 架构是把同一个请求同时发送给多个 agent 实例（例如 5 个或 10 个），让它们各自独立尝试完成任务，agent 之间彼此不通信。（[06:02](https://youtu.be/Mi5wOpAgixw?t=362)）
- 独立式 multi-agent 架构适用的例子：当你对要构建的 UI 只有模糊想法、还不确定具体细节时，可以把需求规格同时交给三个 Claude Code 实例，让它们各自给出不同方案，再从中挑选最佳的一个。（[06:02](https://youtu.be/Mi5wOpAgixw?t=362)）
- 独立式 multi-agent 架构的优点是实现简单，因为 agent 之间不需要任何协调（coordination）机制。（[06:02](https://youtu.be/Mi5wOpAgixw?t=362)）
- 独立式 multi-agent 架构的缺点是各 agent 互不交互，本质上只是把同一个 AI agent 多跑几次，因此相比单 agent 通常只能带来边际（marginal）收益提升。（[06:02](https://youtu.be/Mi5wOpAgixw?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-code]]
- [[google-multi-agent-architecture-paper]]
- [[independent-multi-agent-error-rate]]
- [[voting-aggregation-mechanism]]
%% ytkb:end %%
