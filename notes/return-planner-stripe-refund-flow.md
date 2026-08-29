---
title: Return Planner Stripe Refund Flow
aliases: []
tags:
- concept
summary: 退款流程中 return planner agent 调用 Stripe API 执行支付退款，Stripe API 处理完成后将退款结果返回给
  return planner。
created: '2026-08-26'
updated: '2026-08-26'
---

# Return Planner Stripe Refund Flow

%% ytkb:def %%
退款流程中 return planner agent 调用 Stripe API 执行支付退款，Stripe API 处理完成后将退款结果返回给 return planner。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- return planner agent 完成退款判定后会调用 Stripe API 发起实际的支付退款，Stripe API 处理完成后返回「payment refund done」的确认信息。（[15:04](https://youtu.be/CyLYY_xb5bQ?t=904)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[centralized-agent-architecture]]
%% ytkb:end %%
