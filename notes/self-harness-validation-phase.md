---
title: Self-Harness 提案验证阶段
aliases: []
tags:
- concept
summary: Self-Harness 的第三阶段，对候选 harness 修改在训练集和测试集上做回归测试，只有两边都无性能回退才会被接受合并。
created: '2026-08-26'
updated: '2026-08-26'
---

# Self-Harness 提案验证阶段

%% ytkb:def %%
Self-Harness 的第三阶段，对候选 harness 修改在训练集和测试集上做回归测试，只有两边都无性能回退才会被接受合并。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- 提案验证阶段要求候选修改在训练集和测试集上都不能出现性能回退才会被接受并合并生成新一代 harness，被拒绝的修改只做记录、不会改动现有系统。（[15:08](https://youtu.be/z_F0z7wF5XU?t=908)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[self-harness]]
- [[self-harness-proposal-phase]]
%% ytkb:end %%
