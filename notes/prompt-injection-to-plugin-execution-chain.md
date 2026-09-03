---
title: Prompt Injection to Plugin Execution Chain
aliases: []
tags:
- concept
summary: 攻击者仅需让 AI 读取一段其构造的恶意内容，即可触发 prompt injection 并使模型自主调用官方接口定义、运行恶意插件，全程无需用户点击确认或攻击者窃取任何凭据。
created: '2026-09-03'
updated: '2026-09-03'
---

# Prompt Injection to Plugin Execution Chain

%% ytkb:def %%
攻击者仅需让 AI 读取一段其构造的恶意内容，即可触发 prompt injection 并使模型自主调用官方接口定义、运行恶意插件，全程无需用户点击确认或攻击者窃取任何凭据。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 攻击者不需要提前获取任何权限或凭据，只要让 AI 读取一段其编写的内容即可触发注入攻击。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cordis-define-run-plugin-api]]
- [[unwired-approval-service-vulnerability]]
%% ytkb:end %%
