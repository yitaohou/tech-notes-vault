---
title: Separation of File Metadata and Blob Storage
aliases: []
tags:
- concept
summary: 文件上传架构中，实际文件内容（blob）由 object storage 保存，文件元数据单独存储在关系型数据库中的设计方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Separation of File Metadata and Blob Storage

%% ytkb:def %%
文件上传架构中，实际文件内容（blob）由 object storage 保存，文件元数据单独存储在关系型数据库中的设计方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-file-storage]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 文件上传架构会把文件本体（blob）与文件元数据分开存储：file service 收到上传请求后，先在关系型数据库中为该文件生成并保存元数据记录，而不是把文件本体本身存进数据库。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[file-upload-request-flow]]
- [[files-table-schema]]
- [[object-storage]]
%% ytkb:end %%
