---
title: JWT/Bearer Token Claims for Authorization
aliases: []
tags:
- concept
summary: 指用户完成身份认证后系统签发的 JWT 或 bearer token 中所携带、用于支撑后续授权判断的具体字段信息。
created: '2026-08-26'
updated: '2026-08-26'
---

# JWT/Bearer Token Claims for Authorization

%% ytkb:def %%
指用户完成身份认证后系统签发的 JWT 或 bearer token 中所携带、用于支撑后续授权判断的具体字段信息。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 用户完成身份认证后，系统通常签发 JWT 或 bearer token，其中携带 user ID、角色（如 admin、editor）、允许访问的 scope、过期时间以及签发者（issuer）等信息，用于支撑后续的授权判断。（[1:51:32](https://youtu.be/oYxTTirKY8M?t=6692)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[authorization-header-token-transport]]
- [[jwt-token-authentication]]
- [[oauth2-delegated-authorization]]
%% ytkb:end %%
