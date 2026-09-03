---
title: DeepSeek Harness VM Sandbox
aliases: []
tags:
- concept
summary: DeepSeek Harness 插件运行所依赖的沙箱机制，基于 Node.js 内置 vm 模块在当前进程内部划出隔离区域运行不可信代码，而非完整操作系统级虚拟机。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness VM Sandbox

%% ytkb:def %%
DeepSeek Harness 插件运行所依赖的沙箱机制，基于 Node.js 内置 vm 模块在当前进程内部划出隔离区域运行不可信代码，而非完整操作系统级虚拟机。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 该沙箱是在 Harness 插件代码所运行的 Node.js 进程内部划出一块隔离区域，让不可信任的代码（如插件代码）在其中运行而不能触及外部，设计上插件不能直接访问主机，只能通过指定接口调用宿主服务。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[execute-agent-context-leak]]
- [[isolated-execution-environment]]
%% ytkb:end %%
