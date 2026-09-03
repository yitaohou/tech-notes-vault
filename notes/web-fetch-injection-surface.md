---
title: Web Fetch Large Injection Surface
aliases: []
tags:
- concept
summary: 指 web fetch 因把整页原始内容原样喂给 AI，而网页内容来源不可控，导致其注入面远大于只返回摘要的 web search 的风险特征。
created: '2026-09-03'
updated: '2026-09-03'
---

# Web Fetch Large Injection Surface

%% ytkb:def %%
指 web fetch 因把整页原始内容原样喂给 AI，而网页内容来源不可控，导致其注入面远大于只返回摘要的 web search 的风险特征。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- web search 只返回结果摘要注入面较小，而 web fetch 把整页所有原始内容原样喂给 AI，网页是别人地盘、内容完全未知，如果确实需要抓取原始网页，应先确认机器是否能访问到内网敏感服务，若能访问则尽量不要安装该工具。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-web-fetch-tool]]
- [[deepseek-harness-web-search-tool]]
%% ytkb:end %%
