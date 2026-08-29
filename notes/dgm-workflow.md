---
title: DGM Workflow
aliases: []
tags:
- concept
summary: DGM 的具体运行逻辑：从单一初始 agent 出发，反复选择父代、生成新版本并评估后加入种群。
created: '2026-08-26'
updated: '2026-08-26'
---

# DGM Workflow

%% ytkb:def %%
DGM 的具体运行逻辑：从单一初始 agent 出发，反复选择父代、生成新版本并评估后加入种群。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- DGM 从种群中只有一个编码 agent 开始，按性能正比、后代数量反比的概率选择父 agent，令其检查自身基准测试日志并提出对自己 Harness 代码库的改进，生成新版本 agent。（[18:11](https://youtu.be/z_F0z7wF5XU?t=1091)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[darwin-godel-machine]]
- [[dgm-parent-selection]]
%% ytkb:end %%
