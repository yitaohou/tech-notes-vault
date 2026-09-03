---
title: .dsh API Key File Permission Check
aliases: []
tags:
- concept
summary: DeepSeek Harness 启动时对存放在 .dsh 文件夹内的 API 密钥文件权限进行的自动检查机制。
created: '2026-09-03'
updated: '2026-09-03'
---

# .dsh API Key File Permission Check

%% ytkb:def %%
DeepSeek Harness 启动时对存放在 .dsh 文件夹内的 API 密钥文件权限进行的自动检查机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek API 密钥存放在 .dsh 文件夹内的一个文件中，DeepSeek Harness 启动时会自动检查该文件权限，权限过松会报错并提示收紧，可用 chmod 600（修改文件权限的命令）来修正。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dsh-hidden-config-folder]]
%% ytkb:end %%
