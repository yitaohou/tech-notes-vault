---
title: File Metadata and Object Storage Split
aliases: []
tags:
- concept
summary: 文件实际内容存放在 object storage，而文件的元数据（如通过 ID 查询得到的 URL）存放在关系型数据库中的分离式存储设计。
created: '2026-08-26'
updated: '2026-08-26'
---

# File Metadata and Object Storage Split

%% ytkb:def %%
文件实际内容存放在 object storage，而文件的元数据（如通过 ID 查询得到的 URL）存放在关系型数据库中的分离式存储设计。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-file-storage]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 获取一个文件时通常分两步：先查关系型数据库拿到文件 ID 对应的 URL（元数据），再去 object storage 用该 URL 取出文件本体。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[cache-aside-pattern]]
- [[dynamodb]]
%% ytkb:end %%
