---
title: Policy Check Gate Before Tool Call
aliases: []
tags:
- concept
summary: 指 agent 在触发功能性 API 调用之前，先完成 RAG 检索与政策比对，只有确认符合政策后才进入下一步执行动作的决策流程。
created: '2026-08-26'
updated: '2026-08-26'
---

# Policy Check Gate Before Tool Call

%% ytkb:def %%
指 agent 在触发功能性 API 调用之前，先完成 RAG 检索与政策比对，只有确认符合政策后才进入下一步执行动作的决策流程。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- return planner agent 会先完成 RAG 政策检索与 guardrails 比对，确认符合政策后才触发具体功能调用（如 Shopify API 处理退货），形成先检查后执行的决策链路。（[14:10](https://youtu.be/CyLYY_xb5bQ?t=850)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agentic-write-actions]]
- [[guardrails-policy-alignment-check]]
- [[retrieval-augmented-generation]]
%% ytkb:end %%
