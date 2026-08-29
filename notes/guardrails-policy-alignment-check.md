---
title: Guardrails Policy Alignment Check
aliases: []
tags:
- concept
summary: 把政策文本传入 guardrails 服务，对 agent 即将采取的行动做是否符合政策的二次校验机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# Guardrails Policy Alignment Check

%% ytkb:def %%
把政策文本传入 guardrails 服务，对 agent 即将采取的行动做是否符合政策的二次校验机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 可以把退货政策文本传给 guardrails 服务，让其对 RAG 检索出的信息做二次比对，判断是否符合公司政策，再决定是否通知 agent 继续执行。（[13:05](https://youtu.be/CyLYY_xb5bQ?t=785)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-safety-oversight]]
- [[retrieval-augmented-generation]]
%% ytkb:end %%
