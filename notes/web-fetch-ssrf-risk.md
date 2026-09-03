---
title: Web Fetch SSRF Risk
aliases: []
tags:
- concept
summary: 指 web fetch 工具因缺乏内网防控，可被诱导访问其宿主机器本不应访问的内部网络地址的风险，即 SSRF（服务端请求伪造）。
created: '2026-09-03'
updated: '2026-09-03'
---

# Web Fetch SSRF Risk

%% ytkb:def %%
指 web fetch 工具因缺乏内网防控，可被诱导访问其宿主机器本不应访问的内部网络地址的风险，即 SSRF（服务端请求伪造）。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- web fetch 没有内网防控，机器能访问什么它就能访问什么，例如家里远程连公司内网、云服务器上的内部网络都可能被摸到，这类行为的学名是 SSRF（服务端请求伪造），即诱导工具访问其本不应访问的内网地址。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-web-fetch-tool]]
%% ytkb:end %%
