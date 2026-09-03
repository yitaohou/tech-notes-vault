---
title: Empirical Failure-Driven Prompt Diagnosis
aliases: []
tags:
- concept
summary: 一种确定AI设定该如何补强的方法论：先让模型执行一个足够难、且是真实工作会用到的任务，配合检查结果的方法，观察它反复失败的地方，再据此决定该补充Prompt、加一个Skill，还是接上MCP以获取缺少的资料和工具。
created: '2026-09-03'
updated: '2026-09-03'
---

# Empirical Failure-Driven Prompt Diagnosis

%% ytkb:def %%
一种确定AI设定该如何补强的方法论：先让模型执行一个足够难、且是真实工作会用到的任务，配合检查结果的方法，观察它反复失败的地方，再据此决定该补充Prompt、加一个Skill，还是接上MCP以获取缺少的资料和工具。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-prompt-engineering]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Z-4AsgTYv2c %%
### 来自 [[2026-09-02-claude-code-之父建議每六個月刪光你的-claudemd]]
- Boris 认为与其把网络上看到的各种技巧全部塞进设定，不如先让模型执行一个真实且够难的任务，观察它反复失败的地方，再据此决定要补充 Prompt、加 Skill，还是接上 MCP。（[12:47](https://youtu.be/Z-4AsgTYv2c?t=767)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[boris-cherny]]
- [[claude-skills]]
- [[model-context-protocol]]
%% ytkb:end %%
