---
title: DeepSeek Harness Read-Only Mode Read Leak
aliases: []
tags:
- concept
summary: DeepSeek Harness 中一种只拦截写操作、不拦截读操作的安全缺陷，导致开启只读模式后 AI 仍可读取工作区外的敏感文件并将内容外发。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Read-Only Mode Read Leak

%% ytkb:def %%
DeepSeek Harness 中一种只拦截写操作、不拦截读操作的安全缺陷，导致开启只读模式后 AI 仍可读取工作区外的敏感文件并将内容外发。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 很多人处理不可信项目时会切换到只读模式、认为这样就安全，但验证发现只读模式下 AI 写文件会被文件系统权限拒绝，读取工作区外的文件（如 SSH 私钥、保存密码密钥的环境变量）却能成功，且读到的内容还可以被发送到外部服务器，说明只读模式不限制查看权限。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-config-code-execution]]
%% ytkb:end %%
