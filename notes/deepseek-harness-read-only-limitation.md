---
title: DeepSeek Harness Read-Only Mode Read Access Limitation
aliases: []
tags:
- concept
summary: 指 DeepSeek Harness 的 read-only 模式只拦截写入操作、不拦截读取操作的局限性。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Read-Only Mode Read Access Limitation

%% ytkb:def %%
指 DeepSeek Harness 的 read-only 模式只拦截写入操作、不拦截读取操作的局限性。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- read-only 模式只拦截写入而不拦截读取，AI 依然能读取机器上的文件，包括本地存储的密钥。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-read-only-mode]]
%% ytkb:end %%
