---
title: Static Analysis Bloat Blindspot
aliases: []
tags:
- concept
summary: 指静态分析工具即使代码文件非常臃肿庞大也可能显示全部通过，无法单靠静态分析发现这类问题。
created: '2026-08-26'
updated: '2026-08-26'
---

# Static Analysis Bloat Blindspot

%% ytkb:def %%
指静态分析工具即使代码文件非常臃肿庞大也可能显示全部通过，无法单靠静态分析发现这类问题。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-code-quality-tooling]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 静态分析（static analysis）即便代码文件极度臃肿庞大也可能全部检查通过，因此不能仅依赖它来发现过大文件的问题，还需要通过为其编写单元测试来倒逼拆分。（[09:01](https://youtu.be/AMerB8XjfZ0?t=541)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-monolithic-component-antipattern]]
- [[component-file-length-analysis]]
%% ytkb:end %%
