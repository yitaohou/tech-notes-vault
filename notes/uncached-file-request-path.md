---
title: Uncached File Request Path
aliases: []
tags:
- concept
summary: 未引入缓存前，一次获取文件请求需要完整经过的处理路径：客户端到 gateway，gateway 到 files service 查询关系型数据库获得元数据，再到
  object storage 取文件，最终把结果携带元数据一起返回给 gateway。
created: '2026-08-26'
updated: '2026-08-26'
---

# Uncached File Request Path

%% ytkb:def %%
未引入缓存前，一次获取文件请求需要完整经过的处理路径：客户端到 gateway，gateway 到 files service 查询关系型数据库获得元数据，再到 object storage 取文件，最终把结果携带元数据一起返回给 gateway。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-file-storage]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 未加缓存前完整的文件获取路径是：gateway 转发请求给 files service，files service 查询 relational database 获取文件元数据，再访问 object storage 取回实际文件，最终把附带元数据的文件返回给 gateway。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[caching-motivation-repeated-access]]
%% ytkb:end %%
