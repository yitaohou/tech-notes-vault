---
title: DeepSeek Harness Three-Tier Sandbox
aliases: []
tags:
- concept
summary: DeepSeek Harness 的安全设计，将沙箱隔离级别分为只读、工作区可写、完全放开三档，用以限制 AI 能访问的文件和资源范围。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Three-Tier Sandbox

%% ytkb:def %%
DeepSeek Harness 的安全设计，将沙箱隔离级别分为只读、工作区可写、完全放开三档，用以限制 AI 能访问的文件和资源范围。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 三层沙箱默认选项是工作区可写，即 AI 只能修改用户指定工作文件夹内的内容；只读档只能查看文件不能修改；完全放开档可访问电脑上所有文件，切换该模式时需要二次确认。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[code-execution-sandboxing]]
- [[isolated-execution-environment]]
%% ytkb:end %%
