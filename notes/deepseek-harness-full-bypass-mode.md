---
title: DeepSeek Harness Full Bypass Mode
aliases: []
tags:
- concept
summary: DeepSeek Harness 中的完全放开权限策略，AI 执行任何操作都不会询问用户确认。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Full Bypass Mode

%% ytkb:def %%
DeepSeek Harness 中的完全放开权限策略，AI 执行任何操作都不会询问用户确认。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 完全放开模式下 AI 做任何操作都不会询问用户，启动这一档相当于撤掉所有权限控制，对应攻击链第三步「滥用运行插件的接口」，各类高危操作（如删除整个系统、删除磁盘）都可能由此模式引发，不应轻易启动。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[yolo-mode-claude-code]]
%% ytkb:end %%
