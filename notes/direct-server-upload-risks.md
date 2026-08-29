---
title: Risks of Direct File Upload to Own Server
aliases: []
tags:
- concept
summary: 指将文件直接流式上传到自己服务器时存在的风险，包括超时和潜在的恶意攻击。
created: '2026-08-26'
updated: '2026-08-26'
---

# Risks of Direct File Upload to Own Server

%% ytkb:def %%
指将文件直接流式上传到自己服务器时存在的风险，包括超时和潜在的恶意攻击。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-file-upload]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 不应该把文件直接流式上传到自己的服务器：一是服务器可能无法承受大体积数据流并因此触发 timeout，二是直接接收上传数据会增加遭受恶意攻击的风险，绕开这种方式有助于提前预防这类攻击。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[database-unsuitable-for-large-files]]
- [[object-storage]]
%% ytkb:end %%
