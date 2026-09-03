---
title: DeepSeek Harness Management Port Default Config
aliases: []
tags:
- concept
summary: DeepSeek Harness 管理界面默认只监听本机回环地址 127.0.0.1 的 3080 端口，外部设备默认无法连接。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Management Port Default Config

%% ytkb:def %%
DeepSeek Harness 管理界面默认只监听本机回环地址 127.0.0.1 的 3080 端口，外部设备默认无法连接。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek Harness 的管理界面默认只监听本机回环地址127.0.0.1的3080端口，在此状态下外部设备根本连接不上，此前提到的远程打法在默认配置下走不通。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-port-exposure-risks]]
%% ytkb:end %%
