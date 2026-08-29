---
title: Object Storage Bypasses API Server
aliases: []
tags:
- concept
summary: 通过让客户端直接上传文件到对象存储而非经过应用服务器，完全绕开应用服务器，从而避免服务器被上传请求压垮。
created: '2026-08-26'
updated: '2026-08-26'
---

# Object Storage Bypasses API Server

%% ytkb:def %%
通过让客户端直接上传文件到对象存储而非经过应用服务器，完全绕开应用服务器，从而避免服务器被上传请求压垮。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-file-upload]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 使用 presigned URL 直接上传到对象存储后，应用服务器完全不会被上传流量触及，从根本上解决了文件服务被上传请求压垮变慢的问题。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[presigned-url-direct-upload]]
%% ytkb:end %%
