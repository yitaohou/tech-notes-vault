---
title: Workspace Secrets Exfiltration Risk
aliases: []
tags:
- concept
summary: 密钥、密码、证件等敏感信息若放在 AI coding agent 的工作区内，一旦被 AI 读取到就有被发送出去的风险，一旦泄露就完全脱离用户的掌控。
created: '2026-09-03'
updated: '2026-09-03'
---

# Workspace Secrets Exfiltration Risk

%% ytkb:def %%
密钥、密码、证件等敏感信息若放在 AI coding agent 的工作区内，一旦被 AI 读取到就有被发送出去的风险，一旦泄露就完全脱离用户的掌控。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 密钥、密码、证件类敏感文件不应放入 AI agent 的工作区，因为 AI 一旦读到这些内容就有可能将其发出去，导致完全脱离用户掌控。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[credentials-yaml-plaintext-storage]]
%% ytkb:end %%
