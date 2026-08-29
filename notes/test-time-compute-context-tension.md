---
title: Test-Time Compute 与 Context Rot 的矛盾
aliases: []
tags:
- concept
summary: 指 test-time compute scaling（更多 token 带来更好表现）与 context rot（上下文窗口填得越满表现越差）之间存在的张力。
created: '2026-08-26'
updated: '2026-08-26'
---

# Test-Time Compute 与 Context Rot 的矛盾

%% ytkb:def %%
指 test-time compute scaling（更多 token 带来更好表现）与 context rot（上下文窗口填得越满表现越差）之间存在的张力。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Mi5wOpAgixw %%
### 来自 [[2026-02-22-multi-agent-systems-explained-in-17-minutes]]
- 存在一个核心矛盾：更多 token 能提升 agent 表现（test-time compute scaling），但上下文窗口填得越满又会因 context rot 导致表现下降，如何兼得两者是关键问题。（[00:00](https://youtu.be/Mi5wOpAgixw?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[context-rot]]
- [[multi-agent-systems]]
- [[test-time-compute-scaling]]
%% ytkb:end %%
