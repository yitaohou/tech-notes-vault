---
title: DeepSeek Harness Permission Tiers
aliases: []
tags:
- concept
summary: DeepSeek Harness 的权限体系被划分为三个档位：只读工作区、工作区可写、完全放开。
created: '2026-09-03'
updated: '2026-09-04'
---

# DeepSeek Harness Permission Tiers

%% ytkb:def %%
DeepSeek Harness 的权限体系被划分为三个档位：只读工作区、工作区可写、完全放开。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek Harness 的权限自分为三档，分别是只读工作区、工作区可写和完全放开，用户可根据需要在这三档之间切换配置。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
%% ytkb:end %%

%% ytkb:video:buYQ-_V2Wv0 %%
### 来自 [[2026-09-04-一个视频搞懂deepseek-harness]]
- 只读和工作区可写这两档权限下，即使只是读取一个文件也需要用户手动停下确认，使用体验较为繁琐；而完全访问档虽然自由，但网上已出现因权限过大导致文件被一键删光的真实受害案例。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-default-workspace-writable]]
- [[dsh-approval-gate-plugin]]
%% ytkb:end %%
