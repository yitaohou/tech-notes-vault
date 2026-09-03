---
title: File Permission (chmod 600) AI Bypass
aliases: []
tags:
- concept
summary: 官方文档承认的局限：给密钥文件设置 chmod 600 权限只能阻挡同一台电脑上的其他用户读取，无法阻挡以用户自身身份运行的 AI 读取该文件。
created: '2026-09-03'
updated: '2026-09-03'
---

# File Permission (chmod 600) AI Bypass

%% ytkb:def %%
官方文档承认的局限：给密钥文件设置 chmod 600 权限只能阻挡同一台电脑上的其他用户读取，无法阻挡以用户自身身份运行的 AI 读取该文件。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 官方文档说明文件权限设置能挡住同一台电脑上的其他用户，但挡不住 AI 本身，因为 AI 运行时使用的是用户自己的身份，拥有用户所有的权限。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[credentials-yaml-plaintext-storage]]
%% ytkb:end %%
