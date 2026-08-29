---
title: Basic Client-API-Database Architecture
aliases: []
tags:
- concept
summary: 设计类似 LeetCode 的编程题目系统时采用的基础三层架构：client 发送请求给 API server，API server 再与 database
  交互。
created: '2026-08-26'
updated: '2026-08-26'
---

# Basic Client-API-Database Architecture

%% ytkb:def %%
设计类似 LeetCode 的编程题目系统时采用的基础三层架构：client 发送请求给 API server，API server 再与 database 交互。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 设计编程题目查看系统的基础架构为 client 发送 GET 请求给 API server，API server 再读写 database；这个交互是双向的，因为既要读取题目也要提交解答（submit）。（[21:07](https://youtu.be/QBHTbtWSECg?t=1267)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[dynamodb-choice-for-schema-flexibility]]
- [[problem-entity-schema-design]]
%% ytkb:end %%
