---
title: DeepSeek Harness Approval Fail-Close Design
aliases: []
tags:
- concept
summary: DeepSeek Harness 的审批机制设计，对高风险操作弹出卡片要求用户确认，并采用 fail-close 原则：审批服务出错或无人应答时一律视为拒绝。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Approval Fail-Close Design

%% ytkb:def %%
DeepSeek Harness 的审批机制设计，对高风险操作弹出卡片要求用户确认，并采用 fail-close 原则：审批服务出错或无人应答时一律视为拒绝。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 审批机制遵循 fail-close 原则，即审批流程出现异常或超时无响应时默认拒绝执行，而不是默认放行。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[agentic-write-actions]]
- [[human-approval-for-impactful-actions]]
%% ytkb:end %%
