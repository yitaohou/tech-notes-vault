---
title: Sequential Task Single-Agent Advantage
aliases: []
tags:
- concept
summary: 当任务需要按顺序执行——先执行动作、获取信息，再根据新信息更新计划或执行下一步——时，单代理系统比多代理系统更有效。
created: '2026-08-26'
updated: '2026-08-26'
---

# Sequential Task Single-Agent Advantage

%% ytkb:def %%
当任务需要按顺序执行——先执行动作、获取信息，再根据新信息更新计划或执行下一步——时，单代理系统比多代理系统更有效。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Mi5wOpAgixw %%
### 来自 [[2026-02-22-multi-agent-systems-explained-in-17-minutes]]
- 如果任务是顺序性的（执行、获取信息、再据此更新计划或执行下一步），单代理系统效果优于多代理系统。（[03:02](https://youtu.be/Mi5wOpAgixw?t=182)）
- 举例说明顺序任务：先查阅 Chroma DB 最新文档，再据此写出 PRD/计划，最后才能构建应用，三步必须严格按顺序完成，无法并行。（[03:20](https://youtu.be/Mi5wOpAgixw?t=200)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[decomposable-task-multi-agent-advantage]]
%% ytkb:end %%
