---
title: Agent Memory Hierarchy
aliases: []
tags:
- concept
summary: 指agent系统中根据信息重要性和使用频率，将信息分别写入模型训练权重、长期记忆（如 RAG）与短期记忆（会话内即时上下文）的三层划分方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Agent Memory Hierarchy

%% ytkb:def %%
指agent系统中根据信息重要性和使用频率，将信息分别写入模型训练权重、长期记忆（如 RAG）与短期记忆（会话内即时上下文）的三层划分方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 对所有任务都必需的信息应该通过训练直接写入模型权重，很少用到的信息应放在长期记忆（如 RAG）中，而当前会话的即时上下文信息则属于短期记忆。（[42:04](https://youtu.be/JV3pL1_mn2M?t=2524)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[retrieval-augmented-generation]]
%% ytkb:end %%
