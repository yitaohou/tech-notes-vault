---
title: DeepSeek Harness Sandbox OS-Level Implementation
aliases: []
tags:
- concept
summary: DeepSeek Harness 三层沙箱在不同操作系统上分别复用系统自带隔离机制实现：Linux 用 bwrap 加 landlock，macOS
  用 sandbox，Windows 用受限令牌。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Sandbox OS-Level Implementation

%% ytkb:def %%
DeepSeek Harness 三层沙箱在不同操作系统上分别复用系统自带隔离机制实现：Linux 用 bwrap 加 landlock，macOS 用 sandbox，Windows 用受限令牌。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 三层沙箱的底层实现按操作系统区分，分别调用 Linux、macOS、Windows 各自系统自带的隔离机制，而非自行重新造轮子。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-three-tier-sandbox]]
%% ytkb:end %%
