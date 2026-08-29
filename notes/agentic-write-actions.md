---
title: Agentic Write Actions
aliases: []
tags:
- concept
summary: agentic 系统中会对外部环境产生实际改变的动作，例如发送邮件、下单、发起转账，能大幅提升系统能力但也带来重大风险，需要格外谨慎并配备相应安全机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# Agentic Write Actions

%% ytkb:def %%
agentic 系统中会对外部环境产生实际改变的动作，例如发送邮件、下单、发起转账，能大幅提升系统能力但也带来重大风险，需要格外谨慎并配备相应安全机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- write actions（如发邮件、下单、转账）会让 agent 系统直接改变外部环境状态，因此比只读操作风险大得多，实施时需要额外的谨慎和安全防护。（[72:08](https://youtu.be/JV3pL1_mn2M?t=4328)）
%% ytkb:end %%

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 退货流程中，planner agent 在确认符合政策后会触发 Shopify API 执行 return，这是一个会对外部系统产生实际改变的 write action。（[14:35](https://youtu.be/CyLYY_xb5bQ?t=875)）
- 以 CRM 系统为例，agent 的 write action 工具可以拉取或写入 deal pipeline 数据，或为内部团队创建、更新 tickets 来管理相关业务流程。（[18:05](https://youtu.be/CyLYY_xb5bQ?t=1085)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agent-tools-power]]
- [[coding-agent]]
- [[multi-agent-system]]
- [[policy-check-gate-before-tool-call]]
%% ytkb:end %%
