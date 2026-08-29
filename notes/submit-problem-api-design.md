---
title: Submit Problem API Design
aliases: []
tags:
- concept
summary: 在线判题类系统中用于提交代码的 POST API 设计，通常包含 problem ID、submission 中的 code 和 language
  字段。
created: '2026-08-26'
updated: '2026-08-26'
---

# Submit Problem API Design

%% ytkb:def %%
在线判题类系统中用于提交代码的 POST API 设计，通常包含 problem ID、submission 中的 code 和 language 字段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 提交问题的 API 设计为 POST 请求，需要 problem ID，submission 中包含 code（字符串类型）和 language（字符串类型）两个字段。（[18:07](https://youtu.be/QBHTbtWSECg?t=1087)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[code-as-string-payload]]
%% ytkb:end %%
