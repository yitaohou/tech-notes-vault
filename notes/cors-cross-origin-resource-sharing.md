---
title: CORS (Cross-Origin Resource Sharing)
aliases: []
tags:
- concept
summary: 一种安全机制，用于控制哪些域名可以从浏览器发起请求调用你的 API，防止恶意网站冒用用户浏览器发起未授权请求。
created: '2026-08-26'
updated: '2026-08-26'
---

# CORS (Cross-Origin Resource Sharing)

%% ytkb:def %%
一种安全机制，用于控制哪些域名可以从浏览器发起请求调用你的 API，防止恶意网站冒用用户浏览器发起未授权请求。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 若 API 仅供自己的前端域名（如 app.yourdomain.com）调用，则应配置 CORS 只允许该来源的请求，来自其他域名（如 app.anotherdomain.com）的请求应被拒绝。（[1:57:34](https://youtu.be/oYxTTirKY8M?t=7054)）
%% ytkb:end %%
