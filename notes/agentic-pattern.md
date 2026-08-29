---
title: Agentic Pattern
aliases: []
tags:
- concept
summary: 让模型主动使用网页搜索、API 等工具去获取信息的模式，与 RAG 相对，是为模型提供额外信息的两大主流模式之一。
created: '2026-08-26'
updated: '2026-08-26'
---

# Agentic Pattern

%% ytkb:def %%
让模型主动使用网页搜索、API 等工具去获取信息的模式，与 RAG 相对，是为模型提供额外信息的两大主流模式之一。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- 为模型提供所需信息主要有两种主流模式：RAG 让模型从外部数据源检索相关信息，agentic pattern 让模型主动使用网页搜索、API 等工具去获取信息。（[30:02](https://youtu.be/JV3pL1_mn2M?t=1802)）
- RAG 主要用于构建上下文（context construction），而 agentic pattern 能做的事情比 RAG 更多。（[30:02](https://youtu.be/JV3pL1_mn2M?t=1802)）
- Agentic pattern 是比 RAG 这类被动检索更主动的方式，它让 AI 主动与外部工具和 API 交互来完成任务，目前仍是快速演进中的实验性领域。（[36:03](https://youtu.be/JV3pL1_mn2M?t=2163)）
- 前面提到的表格数据 RAG 示例本质上是一个简单的 agent，它具有生成 SQL 查询、执行查询、生成回答这三个动作。（[36:03](https://youtu.be/JV3pL1_mn2M?t=2163)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[coding-agent]]
- [[retrieval-augmented-generation]]
- [[text-to-sql-rag]]
%% ytkb:end %%
