---
title: Manual Review Trigger for Config/Dependency Changes
aliases: []
tags:
- concept
summary: 当 AI 改动全局配置、测试、linter、type checker 或 package.json（依赖）等文件时，需要触发人工手动审查。
created: '2026-08-26'
updated: '2026-08-26'
---

# Manual Review Trigger for Config/Dependency Changes

%% ytkb:def %%
当 AI 改动全局配置、测试、linter、type checker 或 package.json（依赖）等文件时，需要触发人工手动审查。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 只要 AI 改动了全局 config、测试、linter、type checker 或 package.json（即新增依赖）等文件，就必须进行人工手动审查；其余组件级改动若已有合适的规范（widgets）把关则无需逐个检查。（[06:00](https://youtu.be/AMerB8XjfZ0?t=360)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[blast-radius-dependency-change]]
%% ytkb:end %%
