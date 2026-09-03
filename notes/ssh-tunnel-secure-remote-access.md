---
title: SSH Tunnel for Secure Remote Access
aliases: []
tags:
- concept
summary: 通过在本机发起加密的 SSH 隧道连接，把远程机器上未对外暴露的端口安全地映射到本地使用的远程访问方式。
created: '2026-09-03'
updated: '2026-09-03'
---

# SSH Tunnel for Secure Remote Access

%% ytkb:def %%
通过在本机发起加密的 SSH 隧道连接，把远程机器上未对外暴露的端口安全地映射到本地使用的远程访问方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 若确实需要远程访问 DeepSeek Harness 管理界面，推荐做法是走 SSH 隧道：在自己电脑上发起加密连接，把远程3080端口映射回本地使用，而不直接把端口暴露到公网。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-port-exposure-risks]]
%% ytkb:end %%
