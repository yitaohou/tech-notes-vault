---
title: 插件即代码的风险等价性
aliases: []
tags:
- concept
summary: 插件能执行的操作（读写文件、联网、启动进程）与普通代码完全相同，区别只在于插件代码是他人所写、用户并不了解其具体行为。
created: '2026-09-03'
updated: '2026-09-03'
---

# 插件即代码的风险等价性

%% ytkb:def %%
插件能执行的操作（读写文件、联网、启动进程）与普通代码完全相同，区别只在于插件代码是他人所写、用户并不了解其具体行为。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 插件能做的事和正常代码完全一样，包括读写文件、联网、启动进程，唯一区别是插件代码是别人写的，用户并不知道它具体做了什么。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-code-as-temporary-plugin]]
%% ytkb:end %%
