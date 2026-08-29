---
title: VM-based Isolated Code Execution
aliases: []
tags:
- concept
summary: 使用独立的虚拟机（VM）节点来执行用户提交代码的方案，通过资源隔离降低安全风险和系统崩溃概率。
created: '2026-08-26'
updated: '2026-08-26'
---

# VM-based Isolated Code Execution

%% ytkb:def %%
使用独立的虚拟机（VM）节点来执行用户提交代码的方案，通过资源隔离降低安全风险和系统崩溃概率。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 相比直接在 API 服务器上执行用户代码，采用基于 VM 的隔离节点执行方案能提供更好的 isolation，系统崩溃的可能性也更低。（[24:07](https://youtu.be/QBHTbtWSECg?t=1447)）
- VM-based 执行方案的代价是系统会变得较重（heavy），因为每个 VM 都需要分配独立的 memory 和 CPU 资源，从而增加整体系统复杂度。（[24:07](https://youtu.be/QBHTbtWSECg?t=1447)）
- VM-based 代码执行方案虽然比直接在 API 服务器上执行更安全，但仍存在资源浪费的低效问题，因为每次代码执行都需要独立分配一整套 VM 资源，造成 resource hogging。（[24:07](https://youtu.be/QBHTbtWSECg?t=1447)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[unsafe-api-server-code-execution]]
%% ytkb:end %%
