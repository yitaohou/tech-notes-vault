---
title: Basic Authentication Flow
aliases: []
tags:
- concept
summary: basic authentication 是最简单的一种认证方式：请求资源时先返回 401，随后客户端在请求头中附上 base64 编码的凭据以完成认证。
created: '2026-08-26'
updated: '2026-08-26'
---

# Basic Authentication Flow

%% ytkb:def %%
basic authentication 是最简单的一种认证方式：请求资源时先返回 401，随后客户端在请求头中附上 base64 编码的凭据以完成认证。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- basic authentication 是最简单的认证形式：首次请求资源会收到 401 unauthorized，随后在后续请求中通过 authorization header 携带 base64 编码后的凭据完成认证。（[84:20](https://youtu.be/oYxTTirKY8M?t=5060)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authorization-header-token-transport]]
%% ytkb:end %%
