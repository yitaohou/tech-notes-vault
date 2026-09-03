---
title: DeepSeek Harness Chained Sandbox Escape RCE
aliases: []
tags:
- concept
summary: DeepSeek Harness 中把配置代码执行、只读模式读取泄露、VM 沙箱逃逸三个漏洞串联起来，最终导致沙箱内插件可在主机上执行任意命令的链式漏洞，是披露的四个漏洞中最严重的一个。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Chained Sandbox Escape RCE

%% ytkb:def %%
DeepSeek Harness 中把配置代码执行、只读模式读取泄露、VM 沙箱逃逸三个漏洞串联起来，最终导致沙箱内插件可在主机上执行任意命令的链式漏洞，是披露的四个漏洞中最严重的一个。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 该链式漏洞本身没有产生新的攻击面，而是把前面三个漏洞串联起来，使原本运行在 VM 沙箱里的插件能够直接在主机上执行命令，达成远程命令执行（RCE），性质上比前三个孤立的单点问题更严重。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-config-code-execution]]
- [[deepseek-harness-readonly-mode-read-leak]]
- [[execute-agent-context-leak]]
%% ytkb:end %%
