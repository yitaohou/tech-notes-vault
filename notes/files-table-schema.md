---
title: Files Table Schema Design
aliases: []
tags:
- concept
summary: 用于存储文件元数据的 files 表的最小字段设计，不包含文件本体。
created: '2026-08-26'
updated: '2026-08-26'
---

# Files Table Schema Design

%% ytkb:def %%
用于存储文件元数据的 files 表的最小字段设计，不包含文件本体。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-file-storage]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- files 表的基本 schema 设计包括：自动生成的文件 ID（generated ID）、文件名（file name）、文件大小（size），以及可选的文件类型字段（type，如 PNG），但不存储文件本身。（[27:06](https://youtu.be/Qa-7iWxDz1A?t=1626)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[file-metadata-blob-separation]]
- [[object-storage]]
%% ytkb:end %%
