---
title: Gradient Checkpointing
aliases: []
tags:
- concept
summary: 梯度检查点（也称 activation recomputation）是通过在反向传播时重新计算激活值而非存储它们来降低训练内存占用的技术。
created: '2026-08-26'
updated: '2026-08-26'
---

# Gradient Checkpointing

%% ytkb:def %%
梯度检查点（也称 activation recomputation）是通过在反向传播时重新计算激活值而非存储它们来降低训练内存占用的技术。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-fine-tuning]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- gradient checkpointing（也叫 activation recomputation）通过不存储激活值、而是在需要时重新计算，来降低训练内存需求，代价是增加训练时间。（[45:04](https://youtu.be/JV3pL1_mn2M?t=2704)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[fine-tuning-memory-requirements]]
%% ytkb:end %%
