---
title: Meta-Harness Proposer Agent
aliases: []
tags:
- concept
summary: Meta-Harness中负责基于历史Harness与分数生成新候选Harness的组件，本身是一个编码Agent。
created: '2026-08-26'
updated: '2026-08-26'
---

# Meta-Harness Proposer Agent

%% ytkb:def %%
Meta-Harness中负责基于历史Harness与分数生成新候选Harness的组件，本身是一个编码Agent。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- Meta-Harness中的提案者本身就是一个编码Agent，它用grep、cat等命令读取文件系统中存储的历史执行记录，而不是把所有内容都塞进提示词上下文。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[context-rot]]
- [[meta-harness-outer-loop]]
%% ytkb:end %%
