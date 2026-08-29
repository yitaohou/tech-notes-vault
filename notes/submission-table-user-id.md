---
title: Submission Table User ID Field
aliases: []
tags:
- concept
summary: submission 表中用于把一条提交记录反向映射到具体用户的字段。
created: '2026-08-26'
updated: '2026-08-26'
---

# Submission Table User ID Field

%% ytkb:def %%
submission 表中用于把一条提交记录反向映射到具体用户的字段。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- submission 表如果缺少 user ID 字段，就无法知道某条提交属于哪个用户，这是设计提交表 schema 时必须补齐的关键信息，需要额外添加。（[36:11](https://youtu.be/QBHTbtWSECg?t=2171)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[competition-submission-filtering]]
%% ytkb:end %%
