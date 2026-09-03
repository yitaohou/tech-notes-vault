---
title: DeepSeek Harness Malicious Tool-Call Command Execution
aliases: []
tags:
- concept
summary: 攻击者以已注册的假模型身份，向 DeepSeek Harness 返回工具调用指令，诱导其调用命令行工具在受害者机器上执行任意命令。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Malicious Tool-Call Command Execution

%% ytkb:def %%
攻击者以已注册的假模型身份，向 DeepSeek Harness 返回工具调用指令，诱导其调用命令行工具在受害者机器上执行任意命令。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 利用链第二、三步：攻击者触发一次新的对话让 DeepSeek Harness 连接假模型，随后假模型以工具调用指令的形式先创建对话再下发任务，任务内容是运行一条命令，DeepSeek Harness 按指令调用命令行工具，在受害者机器上以受害者账户权限执行攻击者指定的命令。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-exploit-chain]]
%% ytkb:end %%
