---
title: API Key vs JWT Distinction
aliases: []
tags:
- concept
summary: API key 是不携带任何信息的纯随机字符串，而 JWT 可以在令牌本身中嵌入身份与权限信息，二者在信息承载方式上的根本差异。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Key vs JWT Distinction

%% ytkb:def %%
API key 是不携带任何信息的纯随机字符串，而 JWT 可以在令牌本身中嵌入身份与权限信息，二者在信息承载方式上的根本差异。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- API key 只是随机字符串、不含任何嵌入信息，而 JWT 可以直接携带身份和权限数据，因此使用 API key 时服务器必须额外查库才能得知调用者是谁、拥有什么权限。（[90:23](https://youtu.be/oYxTTirKY8M?t=5423)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-key-authentication]]
- [[jwt-token-authentication]]
%% ytkb:end %%
