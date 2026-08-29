---
title: Object Storage
aliases: []
tags:
- concept
summary: 专门用于存储不常变化的静态文件（如图片、视频）的存储服务，例如 S3 bucket、Google Cloud bucket。
created: '2026-08-26'
updated: '2026-08-26'
---

# Object Storage

%% ytkb:def %%
专门用于存储不常变化的静态文件（如图片、视频）的存储服务，例如 S3 bucket、Google Cloud bucket。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-file-storage]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- Object storage（如 S3 bucket、Google Cloud bucket）是专门用于承载静态文件的存储方案，适合存放不常变化甚至从不变化的大体积文件，如图片和视频。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[database-unsuitable-for-large-files]]
- [[file-metadata-blob-separation]]
%% ytkb:end %%
