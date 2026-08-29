---
title: Meta-Harness Outer Loop
aliases: []
tags:
- concept
summary: Meta-Harness的外层循环流程：初始化一批Harness候选并记录其代码、分数、轨迹，每轮由提案者生成新候选并验证评估，最终输出帕累托最优的Harness。
created: '2026-08-26'
updated: '2026-08-26'
---

# Meta-Harness Outer Loop

%% ytkb:def %%
Meta-Harness的外层循环流程：初始化一批Harness候选并记录其代码、分数、轨迹，每轮由提案者生成新候选并验证评估，最终输出帕累托最优的Harness。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- Meta-Harness的外层循环是：先初始化一批Harness候选，在文件系统中存下每个Harness的代码、分数、运行轨迹；每轮迭代提案者读取历史Harness和对应分数生成新候选，候选通过接口验证后拿去评估，合格的加入池子；迭代结束后输出所有帕累托最优（Pareto optimal）的Harness。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[meta-harness]]
%% ytkb:end %%
