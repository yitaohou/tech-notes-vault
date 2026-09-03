---
title: Cordis Define / Cordis Run Plugin API
aliases: []
tags:
- concept
summary: DeepSeek Harness 官方提供的插件系统接口，包含用于定义插件的 Cordis Define 和用于运行插件的 Cordis Run，支持
  AI 在运行时动态编写代码并注入为临时插件立即执行。
created: '2026-09-03'
updated: '2026-09-03'
---

# Cordis Define / Cordis Run Plugin API

%% ytkb:def %%
DeepSeek Harness 官方提供的插件系统接口，包含用于定义插件的 Cordis Define 和用于运行插件的 Cordis Run，支持 AI 在运行时动态编写代码并注入为临时插件立即执行。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-agent-architecture]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- DeepSeek Harness 中的 AI 可以在线写一段代码、注射成临时插件马上运行，这是官方功能，插件定义接口叫 Cordis Define、运行时接口叫 Cordis Run，框架的核心卖点正是让 AI 能给自己在线写工具。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
- prompt injection 攻击生效后，模型会自主调用 cordis define 定义插件、再调用 cordis run 运行插件，这两个接口是官方提供给 AI 写工具用的正常功能。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness]]
- [[deepseek-harness-chained-sandbox-escape-rce]]
- [[deepseek-harness-vm-sandbox]]
- [[prompt-injection-to-plugin-execution-chain]]
%% ytkb:end %%
