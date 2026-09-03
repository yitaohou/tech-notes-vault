---
title: DeepSeek Harness Same-Machine Access Vulnerability Has No Config Fix
aliases: []
tags:
- concept
summary: 同一台电脑上其他恶意程序可无认证访问 DeepSeek Harness 接口的问题，属于框架自身设计缺陷，配置层面没有开关可以关闭。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Same-Machine Access Vulnerability Has No Config Fix

%% ytkb:def %%
同一台电脑上其他恶意程序可无认证访问 DeepSeek Harness 接口的问题，属于框架自身设计缺陷，配置层面没有开关可以关闭。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 同一台电脑上的其他恶意程序能够无认证访问 DeepSeek Harness 接口，这是框架自身的设计问题，配置层面没有开关能够关掉，目前唯一的应对办法是不要安装来路不明的软件。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-default-localhost-only]]
%% ytkb:end %%
