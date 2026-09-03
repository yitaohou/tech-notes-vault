---
title: Context Object Security Bypass
aliases: []
tags:
- concept
summary: 指插件不经过接口正常调用服务，而是直接把整个上下文对象窃取带走后离开沙箱，导致写边界限制、进程沙箱、文件权限三道防线（均为沙箱内部代码）全部失效，因为代码已经带着上下文离开了沙箱可管辖的范围。
created: '2026-09-03'
updated: '2026-09-03'
---

# Context Object Security Bypass

%% ytkb:def %%
指插件不经过接口正常调用服务，而是直接把整个上下文对象窃取带走后离开沙箱，导致写边界限制、进程沙箱、文件权限三道防线（均为沙箱内部代码）全部失效，因为代码已经带着上下文离开了沙箱可管辖的范围。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek Harness 的权限检查逻辑被安放在服务调用路径的半路而非入口处，插件正常走接口调用服务时会被检查，但直接窃取整个上下文对象绕开该路径就不会被拦截。（[12:04](https://youtu.be/WrwA7FYGPdQ?t=724)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[subprocess-service-host-privilege-escalation]]
- [[vulnerability-chain-composition]]
%% ytkb:end %%
