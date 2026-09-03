---
title: Loopback Binding Does Not Prevent Local Attacks
aliases: []
tags:
- concept
summary: 指服务默认只监听本机回环地址 127.0.0.1 虽能阻挡远程攻击，但由于接口本身没有认证，本机上任何能发起 HTTP 请求的程序依然可以利用该漏洞。
created: '2026-09-03'
updated: '2026-09-03'
---

# Loopback Binding Does Not Prevent Local Attacks

%% ytkb:def %%
指服务默认只监听本机回环地址 127.0.0.1 虽能阻挡远程攻击，但由于接口本身没有认证，本机上任何能发起 HTTP 请求的程序依然可以利用该漏洞。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek Harness 默认只监听本机回环地址 127.0.0.1，外部设备无法直接连入，能挡住远程攻击，但接口缺乏认证的问题依然存在：同一台电脑上任何能向该端口发起 HTTP 请求的程序（不明软件、潜伏的木马、浏览器诱导安装的恶意脚本等）都能利用这个漏洞。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-exposure-methods]]
- [[deepseek-harness-unauthenticated-management-api]]
%% ytkb:end %%
