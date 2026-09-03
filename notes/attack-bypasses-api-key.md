---
title: Attack Bypasses API Key Requirement
aliases: []
tags:
- concept
summary: 指该类利用攻击全程无需窃取或使用受害者的模型 API 密钥，而是直接控制 harness 本身调用哪个模型、执行什么命令。
created: '2026-09-03'
updated: '2026-09-03'
---

# Attack Bypasses API Key Requirement

%% ytkb:def %%
指该类利用攻击全程无需窃取或使用受害者的模型 API 密钥，而是直接控制 harness 本身调用哪个模型、执行什么命令。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 整个攻击过程中，攻击者从未使用过受害者的 DeepSeek API 密钥；他直接控制的是 DeepSeek Harness 该调用哪个模型、执行什么命令，密钥完全被绕过。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-tool-call-command-execution]]
%% ytkb:end %%
