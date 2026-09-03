---
title: DeepSeek Harness Config Code Execution Vulnerability
aliases: []
tags:
- concept
summary: DeepSeek Harness 加载配置文件时会把某个字段值当作 JavaScript 代码直接执行，使原本应为纯数据的配置文件具备携带可执行代码的能力，属于QVD-2026-57410披露的漏洞之一。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Config Code Execution Vulnerability

%% ytkb:def %%
DeepSeek Harness 加载配置文件时会把某个字段值当作 JavaScript 代码直接执行，使原本应为纯数据的配置文件具备携带可执行代码的能力，属于QVD-2026-57410披露的漏洞之一。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek Harness 解析配置文件时，会把某个值当作 JavaScript 代码在加载配置的那一刻直接执行，验证者在配置文件中隐藏一行写文件代码即可让其在 Harness 启动加载配置时立即运行。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
- 该配置代码执行的触发时机极早，发生在沙箱和审批机制尚未初始化之前，因此当时任何防护机制都不会起作用，从外部抄来的配置文件一旦加载，等同于在启动流程中执行了别人写的（可能是恶意的）代码。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-chained-sandbox-escape-rce]]
- [[deepseek-harness-vm-sandbox]]
%% ytkb:end %%
