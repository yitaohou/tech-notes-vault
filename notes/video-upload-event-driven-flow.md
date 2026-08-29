---
title: Video Upload Event-Driven Flow
aliases: []
tags:
- concept
summary: 视频/文件上传架构中的典型流程：客户端经 API gateway 鉴权后，由 metadata 服务创建记录并返回上传 URL，客户端直接上传字节到对象存储，随后下游服务异步消费该上传事件完成后续处理。
created: '2026-08-26'
updated: '2026-08-26'
---

# Video Upload Event-Driven Flow

%% ytkb:def %%
视频/文件上传架构中的典型流程：客户端经 API gateway 鉴权后，由 metadata 服务创建记录并返回上传 URL，客户端直接上传字节到对象存储，随后下游服务异步消费该上传事件完成后续处理。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-file-storage]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 典型上传流程为：客户端经 API gateway 完成鉴权 → metadata 服务创建数据库行并返回 upload URL → 客户端直接把字节上传到 object storage bucket → 缩略图服务异步消费该上传事件，生成预览图并写回结果。（[33:08](https://youtu.be/Qa-7iWxDz1A?t=1988)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[message-broker-necessity]]
- [[presigned-url-direct-upload]]
%% ytkb:end %%
