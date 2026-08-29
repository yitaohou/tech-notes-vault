---
title: Relational Databases Unsuitable for Large Binary Files
aliases: []
tags:
- concept
summary: 关系型数据库不适合直接存储大体积二进制文件（如几百MB的图片、几十GB的视频）的原因说明。
created: '2026-08-26'
updated: '2026-08-26'
---

# Relational Databases Unsuitable for Large Binary Files

%% ytkb:def %%
关系型数据库不适合直接存储大体积二进制文件（如几百MB的图片、几十GB的视频）的原因说明。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-file-storage]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 不应把文件直接上传到关系型数据库中，因为文件可能有200MB的图片甚至20GB的视频那么大，而关系型数据库并不是为存储这类大体积二进制数据设计的。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[direct-server-upload-risks]]
- [[object-storage]]
%% ytkb:end %%
