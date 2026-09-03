---
title: Unsafe Subprocess Spawn Without Sandbox
aliases: []
tags:
- concept
summary: 指插件通过 execute agent context 取得宿主上下文并调用 subprocess/spawn 在主机上直接启动进程，进程权限等同当前登录用户权限，且未经过
  VM 沙箱或进程沙箱隔离的漏洞机制。
created: '2026-09-03'
updated: '2026-09-03'
---

# Unsafe Subprocess Spawn Without Sandbox

%% ytkb:def %%
指插件通过 execute agent context 取得宿主上下文并调用 subprocess/spawn 在主机上直接启动进程，进程权限等同当前登录用户权限，且未经过 VM 沙箱或进程沙箱隔离的漏洞机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 插件跑起来后通过 execute agent context 拿到宿主上下文、取出 subprocess 并用 spawn 在主机上启动进程，该进程权限就是当前登录用户的权限，VM 沙箱、进程沙箱等整条防线都没有参与进来。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[prompt-injection-to-plugin-execution-chain]]
%% ytkb:end %%
