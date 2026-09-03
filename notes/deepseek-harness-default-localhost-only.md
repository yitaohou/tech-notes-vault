---
title: DeepSeek Harness Default Localhost/LAN-Only Web Service
aliases: []
tags:
- concept
summary: DeepSeek Harness 默认配置下其 web 服务只监听本机局域网地址，阻止局域网外其他设备的连接。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Default Localhost/LAN-Only Web Service

%% ytkb:def %%
DeepSeek Harness 默认配置下其 web 服务只监听本机局域网地址，阻止局域网外其他设备的连接。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek Harness 的 web 服务默认只监听本机局域网地址，能挡住局域网内其他设备的连接，但挡不住同一台电脑上的其他程序访问，这个默认值并不绝对安全。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-same-machine-vuln-no-fix]]
%% ytkb:end %%
