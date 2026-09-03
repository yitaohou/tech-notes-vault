---
title: Host Header Localhost Check Bypass
aliases: []
tags:
- concept
summary: 指服务仅通过检查 HTTP 请求头中的 Host 字段是否等于 localhost 来判断请求是否来自本机，这种基于客户端可伪造字段的校验方式存在被绕过的安全风险。
created: '2026-09-03'
updated: '2026-09-03'
---

# Host Header Localhost Check Bypass

%% ytkb:def %%
指服务仅通过检查 HTTP 请求头中的 Host 字段是否等于 localhost 来判断请求是否来自本机，这种基于客户端可伪造字段的校验方式存在被绕过的安全风险。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek Harness 判断某个高权限请求是否来自本机的依据，是检查该 HTTP 请求头中 Host 字段的值是否等于 localhost，而 Host 字段是每个 HTTP 请求都携带、可被伪造的信息。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-management-api-exposure]]
%% ytkb:end %%
