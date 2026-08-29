---
title: Sandboxed Output via Temporary Directory Cleanup
aliases: []
tags:
- concept
summary: 为保障用户代码执行的隔离性与安全性，将容器输出写入临时目录并定期清理的做法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Sandboxed Output via Temporary Directory Cleanup

%% ytkb:def %%
为保障用户代码执行的隔离性与安全性，将容器输出写入临时目录并定期清理的做法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 为了保障用户提交代码执行时的 isolation 和 security，可以让容器把所有输出写入临时目录，并根据设定的时间间隔或提交用户数量定期清理这些临时文件。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[availability-over-consistency-tradeoff]]
%% ytkb:end %%
