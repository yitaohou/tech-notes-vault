---
title: Chat History Relational Storage
aliases: []
tags:
- concept
summary: 指agent系统中为读取用户过往聊天与邮件记录而设计的、基于关系型数据库存储会话历史的方案。
created: '2026-08-26'
updated: '2026-08-26'
---

# Chat History Relational Storage

%% ytkb:def %%
指agent系统中为读取用户过往聊天与邮件记录而设计的、基于关系型数据库存储会话历史的方案。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 为了加载用户此前的聊天记录和邮件，AI 客服系统需要从关系型数据库（relational database）中查询这些历史数据。（[06:00](https://youtu.be/CyLYY_xb5bQ?t=360)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[relational-vs-nosql-selection-heuristic]]
%% ytkb:end %%
