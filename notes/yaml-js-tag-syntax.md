---
title: YAML !!js Tag Syntax
aliases: []
tags:
- concept
summary: YAML 配置文件格式支持一种特殊语法：在值前面写两个感叹号加上 js，构成类似 !!js 的标签形式，可用于触发特殊解析行为。
created: '2026-09-03'
updated: '2026-09-03'
---

# YAML !!js Tag Syntax

%% ytkb:def %%
YAML 配置文件格式支持一种特殊语法：在值前面写两个感叹号加上 js，构成类似 !!js 的标签形式，可用于触发特殊解析行为。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- Harness 的配置文件是 YAML 格式，而 YAML 支持一种特殊语法，即在值前面写两个感叹号加 js，写成 !!js 这样的标签形式，这正是第一个「配置加载任意代码执行」漏洞的利用切入点。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[yaml-config-arbitrary-code-execution-vuln]]
%% ytkb:end %%
