---
title: AlphaEvolve
aliases: []
tags:
- concept
summary: 一个专门的编码 Agent 进化搜索系统，维护候选程序池，用冻结的大模型生成差异补丁来迭代改进程序。
created: '2026-08-26'
updated: '2026-08-26'
---

# AlphaEvolve

%% ytkb:def %%
一个专门的编码 Agent 进化搜索系统，维护候选程序池，用冻结的大模型生成差异补丁来迭代改进程序。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- AlphaEvolve 作为编码 Agent 进化搜索系统，内部维护一个候选程序池，并用参数冻结的大模型生成 diff 补丁来改进程序。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
- AlphaEvolve 的核心流程是反复评估子进程、保留成功的个体，并逐步找到更优的解。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[darwin-godel-machine]]
- [[evolutionary-search]]
- [[shinka-evolve]]
%% ytkb:end %%
