---
title: Config File Backdoor Persistence
aliases: []
tags:
- concept
summary: 一种持久化攻击手法：攻击者获得代码执行权限后修改配置文件、在其中埋入恶意代码，使该代码在程序每次启动加载配置时都会执行，即使重启系统也无法清除。
created: '2026-09-03'
updated: '2026-09-03'
---

# Config File Backdoor Persistence

%% ytkb:def %%
一种持久化攻击手法：攻击者获得代码执行权限后修改配置文件、在其中埋入恶意代码，使该代码在程序每次启动加载配置时都会执行，即使重启系统也无法清除。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 攻击者拿到命令执行权限后可以改写配置文件、埋入恶意代码，之后每次启动 DeepSeek Harness 加载配置时这段代码都会执行，重启电脑无法清除，只要配置文件存在后门就一直存在。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[unsafe-subprocess-spawn-no-sandbox]]
%% ytkb:end %%
