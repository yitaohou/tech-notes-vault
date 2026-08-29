---
title: API Key Security Limitations
aliases: []
tags:
- concept
summary: API key 机制固有的安全局限性，包括泄露后可被任意冒用，以及默认缺乏内置过期时间。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Key Security Limitations

%% ytkb:def %%
API key 机制固有的安全局限性，包括泄露后可被任意冒用，以及默认缺乏内置过期时间。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-authentication-authorization]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- API key 一旦泄露，任何人都可以冒充持有者访问资源，且 API key 默认没有内置过期机制，除非开发者自行实现。（[90:23](https://youtu.be/oYxTTirKY8M?t=5423)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-key-authentication]]
%% ytkb:end %%
