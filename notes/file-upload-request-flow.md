---
title: File Upload Request Flow
aliases: []
tags:
- concept
summary: 文件上传的典型请求流程：客户端携带元数据与文件本体发往 API gateway，再由 gateway 转发给 file service 处理。
created: '2026-08-26'
updated: '2026-08-26'
---

# File Upload Request Flow

%% ytkb:def %%
文件上传的典型请求流程：客户端携带元数据与文件本体发往 API gateway，再由 gateway 转发给 file service 处理。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-file-storage]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 文件上传的典型流程是：客户端向 API gateway 发送请求，其中包含元数据（如文件名、文件大小）以及文件本体（blob，例如图片数据）；gateway 再把这个请求转发给 file service 处理。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[file-metadata-blob-separation]]
- [[object-storage]]
%% ytkb:end %%
