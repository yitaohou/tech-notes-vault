---
title: OAuth 2 Access Token
aliases: []
tags:
- concept
summary: OAuth 2 中的 access token 只用于证明应用被授权访问用户的特定资源（如 Google Drive 文件），并不能证明用户身份。
created: '2026-08-26'
updated: '2026-08-26'
---

# OAuth 2 Access Token

%% ytkb:def %%
OAuth 2 中的 access token 只用于证明应用被授权访问用户的特定资源（如 Google Drive 文件），并不能证明用户身份。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 拿到 access token 后，应用就可以携带该 token 向 Google Drive API 请求文件并返回用户的文件列表，但 token 本身不包含「你是谁」的信息。（[99:28](https://youtu.be/oYxTTirKY8M?t=5968)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[jwt-token-authentication]]
- [[openid-connect]]
%% ytkb:end %%
