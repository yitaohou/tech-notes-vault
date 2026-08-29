---
title: Postman Auth Type Terminology Confusion
aliases: []
tags:
- concept
summary: 指 Postman 在 Authorization 设置界面把 Basic Auth、Digest Auth、API Key、OAuth 等统一称为
  authentication type，导致 authentication method 与 authorization framework 的区别被混淆的现象。
created: '2026-08-26'
updated: '2026-08-26'
---

# Postman Auth Type Terminology Confusion

%% ytkb:def %%
指 Postman 在 Authorization 设置界面把 Basic Auth、Digest Auth、API Key、OAuth 等统一称为 authentication type，导致 authentication method 与 authorization framework 的区别被混淆的现象。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- Postman 在请求的 Authorization 标签页中把 Basic authentication、Digest authentication、API key 等都统一标注为 authentication type，但实际上其中一些属于 authentication method，另一些（如 OAuth）属于 authorization framework，这种命名方式容易让开发者混淆二者的区别。（[87:22](https://youtu.be/oYxTTirKY8M?t=5242)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-key-authentication]]
- [[authentication-vs-authorization]]
- [[basic-authentication]]
- [[digest-authentication]]
%% ytkb:end %%
