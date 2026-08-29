---
title: Code Encoding/Encryption on Submission
aliases: []
tags:
- concept
summary: 提交代码时先对代码字符串进行编码或加密，传输到 compiler 端后再解码，用于保护提交内容的一种设计思路。
created: '2026-08-26'
updated: '2026-08-26'
---

# Code Encoding/Encryption on Submission

%% ytkb:def %%
提交代码时先对代码字符串进行编码或加密，传输到 compiler 端后再解码，用于保护提交内容的一种设计思路。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 可以对提交的代码进行编码和加密处理，之后在 compiler 侧再解码，作为初期方案的一个可扩展点。（[18:07](https://youtu.be/QBHTbtWSECg?t=1087)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[code-as-string-payload]]
%% ytkb:end %%
