---
title: Config Loading Arbitrary Code Execution Vulnerability
aliases: []
tags:
- concept
summary: DeepSeek Harness 披露的第一个漏洞：由于配置文件加载环节存在缺陷，攻击者可以借此在目标系统上任意执行代码。
created: '2026-09-03'
updated: '2026-09-03'
---

# Config Loading Arbitrary Code Execution Vulnerability

%% ytkb:def %%
DeepSeek Harness 披露的第一个漏洞：由于配置文件加载环节存在缺陷，攻击者可以借此在目标系统上任意执行代码。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 第一个漏洞是「配置加载任意代码执行」，即通过操纵 Harness 加载的配置文件即可导致任意代码在目标系统上执行。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-day-one-vulnerability-disclosure]]
- [[yaml-js-tag-syntax]]
%% ytkb:end %%
