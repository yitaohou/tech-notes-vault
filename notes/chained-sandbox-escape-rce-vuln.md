---
title: Chained Sandbox Escape Leading to RCE
aliases: []
tags:
- concept
summary: DeepSeek Harness 披露的第四个漏洞：把前面几个独立漏洞串联组合起来，最终实现远程命令执行（RCE）。
created: '2026-09-03'
updated: '2026-09-03'
---

# Chained Sandbox Escape Leading to RCE

%% ytkb:def %%
DeepSeek Harness 披露的第四个漏洞：把前面几个独立漏洞串联组合起来，最终实现远程命令执行（RCE）。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 第四个漏洞是把前面几个漏洞串联组合而成的链式沙箱逃逸，最终导致远程命令执行（RCE）。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[docker-sandbox-info-leak-vuln]]
- [[remote-code-execution-definition]]
- [[vm-sandbox-escape-vuln]]
%% ytkb:end %%
