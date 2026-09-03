---
title: Credentials YAML Plaintext Storage
aliases: []
tags:
- concept
summary: DeepSeek Harness 把 API 密钥保存在 credentials.yaml 配置文件中，界面上显示打码后的描述符，但磁盘上实际保存的是未加密的明文原始内容。
created: '2026-09-03'
updated: '2026-09-03'
---

# Credentials YAML Plaintext Storage

%% ytkb:def %%
DeepSeek Harness 把 API 密钥保存在 credentials.yaml 配置文件中，界面上显示打码后的描述符，但磁盘上实际保存的是未加密的明文原始内容。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- API 密钥保存在 credentials.yaml 文件中，界面显示的是打码后的描述符，但磁盘上该文件保存的其实是未加密的明文密钥，打开文件即可直接看到。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[file-permission-chmod600-ai-bypass]]
%% ytkb:end %%
