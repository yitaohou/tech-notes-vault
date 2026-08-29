---
title: Presigned URL Direct Upload
aliases: []
tags:
- concept
summary: 服务器不直接接收文件，而是向对象存储（如 Google Cloud Storage）请求一个临时上传链接，返回给客户端后由客户端直接上传文件到 bucket，绕过应用服务器。
created: '2026-08-26'
updated: '2026-08-26'
---

# Presigned URL Direct Upload

%% ytkb:def %%
服务器不直接接收文件，而是向对象存储（如 Google Cloud Storage）请求一个临时上传链接，返回给客户端后由客户端直接上传文件到 bucket，绕过应用服务器。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-file-upload]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 文件上传架构中，服务器可以调用对象存储生成一个 presigned URL，返回给前端后由用户直接上传文件到 bucket，而不经过应用服务器中转。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
- 设计文件/视频上传架构时，客户端应绕过应用后端，凭 metadata 服务返回的 upload URL 直接把字节数据上传到 object storage bucket，避免后端成为传输瓶颈。（[33:08](https://youtu.be/Qa-7iWxDz1A?t=1988)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[message-broker-necessity]]
- [[object-storage-bypass-api-server]]
- [[video-upload-event-driven-flow]]
%% ytkb:end %%
