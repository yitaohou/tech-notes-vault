---
title: Presigned URL Expiry Window
aliases: []
tags:
- concept
summary: 为 presigned upload URL 设置的较短有效期，超过该时间窗口链接即失效，用于降低安全风险。
created: '2026-08-26'
updated: '2026-08-26'
---

# Presigned URL Expiry Window

%% ytkb:def %%
为 presigned upload URL 设置的较短有效期，超过该时间窗口链接即失效，用于降低安全风险。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-file-upload]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 生成的上传链接必须设置很小的有效期窗口（expiry date），以防止链接被滥用。（[30:07](https://youtu.be/Qa-7iWxDz1A?t=1807)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[presigned-url-direct-upload]]
%% ytkb:end %%
