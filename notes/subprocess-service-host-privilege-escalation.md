---
title: Subprocess Service Host Privilege Escalation
aliases: []
tags:
- concept
summary: DeepSeek Harness 中 subprocess 是主机上负责启动系统进程的关键服务，若被沙箱内插件通过窃取的上下文对象调用，命令会以当前登录用户权限在主机（而非沙箱）上执行。
created: '2026-09-03'
updated: '2026-09-03'
---

# Subprocess Service Host Privilege Escalation

%% ytkb:def %%
DeepSeek Harness 中 subprocess 是主机上负责启动系统进程的关键服务，若被沙箱内插件通过窃取的上下文对象调用，命令会以当前登录用户权限在主机（而非沙箱）上执行。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- PoC 让沙箱内插件调用窃取到的 subprocess 服务的 spawn 方法，在主机上成功写入文件并输出「unconfined host process」，证明命令逃逸出沙箱、在主机上以用户权限执行成功。（[12:04](https://youtu.be/WrwA7FYGPdQ?t=724)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[context-object-security-bypass]]
- [[prompt-injection-attack]]
%% ytkb:end %%
