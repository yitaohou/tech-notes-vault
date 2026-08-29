---
title: Rate Limiting Per Endpoint
aliases: []
tags:
- concept
summary: 对不同 API 端点分别设置各自的请求频率限制，而不是对整个 API 使用统一限制的做法。
created: '2026-08-26'
updated: '2026-08-26'
---

# Rate Limiting Per Endpoint

%% ytkb:def %%
对不同 API 端点分别设置各自的请求频率限制，而不是对整个 API 使用统一限制的做法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- rate limiting 可以按端点粒度设置，例如对「/comments」这类端点单独设置更严格的每分钟请求次数限制。（[1:54:33](https://youtu.be/oYxTTirKY8M?t=6873)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[rate-limiting]]
%% ytkb:end %%
