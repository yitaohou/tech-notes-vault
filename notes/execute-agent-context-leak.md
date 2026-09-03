---
title: Execute Agent Context Object Leak
aliases: []
tags:
- concept
summary: DeepSeek Harness 中动态加载的插件被直接赋予未经沙箱过滤和检查的 Execute Agent Context（宿主运行时上下文对象），导致插件可绕过沙箱直接读取宿主机密的漏洞。
created: '2026-09-03'
updated: '2026-09-03'
---

# Execute Agent Context Object Leak

%% ytkb:def %%
DeepSeek Harness 中动态加载的插件被直接赋予未经沙箱过滤和检查的 Execute Agent Context（宿主运行时上下文对象），导致插件可绕过沙箱直接读取宿主机密的漏洞。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 动态加载的插件（程序运行过程中临时装入的插件）被直接传入名为 Execute Agent Context 的上下文对象，该对象存放着宿主程序运行时的各种服务引用和状态，且没有经过沙箱隔离或检查。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
- 验证测试中，评审作者预先在宿主机设置的机密字符串（host secret）被恶意插件通过直接读取传入的 Execute Agent Context 对象成功输出，证明该插件完全绕过了沙箱、直接拿到了宿主内部对象。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-chained-sandbox-escape-rce]]
- [[deepseek-harness-vm-sandbox]]
%% ytkb:end %%
