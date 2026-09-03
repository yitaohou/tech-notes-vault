---
title: DeepSeek Harness Anonymous ID Mechanism
aliases: []
tags:
- concept
summary: DeepSeek Harness 在本机首次连接服务器验证 API 密钥成功后，会生成一串随机的匿名 ID，之后每次请求都携带该 ID，用于服务端追踪同一使用者的历史行为。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Anonymous ID Mechanism

%% ytkb:def %%
DeepSeek Harness 在本机首次连接服务器验证 API 密钥成功后，会生成一串随机的匿名 ID，之后每次请求都携带该 ID，用于服务端追踪同一使用者的历史行为。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 首次用自己申请的 API 密钥连接服务器验证成功后，Harness 会在本机生成一串随机的匿名 ID，单看一条请求无法确认使用者身份，但该 ID 是稳定不变的，服务器会看到同一编号发起的所有请求。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[anonymous-id-deanonymization]]
%% ytkb:end %%
