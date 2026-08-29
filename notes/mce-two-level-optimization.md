---
title: MCE Two-Level Optimization
aliases: []
tags:
- concept
summary: MCE的双层优化结构：内层在给定技能下于训练数据上寻找最优上下文，外层在验证集上寻找表现最好的技能。
created: '2026-08-26'
updated: '2026-08-26'
---

# MCE Two-Level Optimization

%% ytkb:def %%
MCE的双层优化结构：内层在给定技能下于训练数据上寻找最优上下文，外层在验证集上寻找表现最好的技能。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-self-improving-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:z_F0z7wF5XU %%
### 来自 [[2026-07-09-ai自我递归改进先要靠harness工程-lilian-weng最新长文-反馈循环-三个设计模式-核]]
- MCE的优化是双层的：内层在给定技能的前提下于训练数据上搜索最优上下文，外层则在验证集上比较不同技能、挑选性能最好的技能。（[09:06](https://youtu.be/z_F0z7wF5XU?t=546)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[mce-framework]]
%% ytkb:end %%
