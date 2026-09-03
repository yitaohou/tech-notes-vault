---
title: Host Header Spoofing Localhost Bypass
aliases: []
tags:
- concept
summary: 利用 HTTP 请求中 host 字段可由客户端任意改写的特性，伪造成来自 localhost 的本机请求，从而绕过服务端仅凭 host 字段判断请求来源的安全检查。
created: '2026-09-03'
updated: '2026-09-03'
---

# Host Header Spoofing Localhost Bypass

%% ytkb:def %%
利用 HTTP 请求中 host 字段可由客户端任意改写的特性，伪造成来自 localhost 的本机请求，从而绕过服务端仅凭 host 字段判断请求来源的安全检查。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek Harness 通过检查请求的 host 字段是否为 localhost 来判断请求是否来自本机，但 host 字段完全由客户端填写，攻击者从外网发起请求并把 host 改成 localhost，即可让服务端把外部请求当成本机请求处理，导致本机检查完全失效。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness]]
- [[deepseek-harness-unauthenticated-management-api]]
%% ytkb:end %%
