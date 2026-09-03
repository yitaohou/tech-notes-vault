---
title: Hidden Text Prompt Injection Technique
aliases: []
tags:
- concept
summary: 一种隐藏提示注入指令的具体手法，把恶意文字用白色写在白色背景上，或藏在文件元数据中，使人类肉眼浏览时不会察觉，但 AI 读取网页/文档源码时能够看到并执行。
created: '2026-09-03'
updated: '2026-09-03'
---

# Hidden Text Prompt Injection Technique

%% ytkb:def %%
一种隐藏提示注入指令的具体手法，把恶意文字用白色写在白色背景上，或藏在文件元数据中，使人类肉眼浏览时不会察觉，但 AI 读取网页/文档源码时能够看到并执行。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 人类正常浏览网页很少会打开开发者工具查看源码，而 AI 读取网页本质就是读取源码，因此隐藏在源码或元数据中的提示注入指令对人不可见、对 AI 却完全可见。（[12:04](https://youtu.be/WrwA7FYGPdQ?t=724)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[prompt-injection-attack]]
%% ytkb:end %%
