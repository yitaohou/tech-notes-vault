---
title: Rate Limiting
aliases: []
tags:
- concept
summary: 限制客户端在给定时间窗口内可发起请求数量的机制，用于防止资源被恶意或过度消耗。
created: '2026-08-26'
updated: '2026-08-26'
---

# Rate Limiting

%% ytkb:def %%
限制客户端在给定时间窗口内可发起请求数量的机制，用于防止资源被恶意或过度消耗。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- 系统开始扩展规模时必须设置 rate limiting，否则恶意用户可能借机耗尽基础设施资源，造成资源浪费、增加成本并影响其他正常用户的体验。（[42:09](https://youtu.be/Qa-7iWxDz1A?t=2529)）
- rate limiting 通常在 API gateway 层或云服务商基础设施层实现，通过识别用户 IP 或其他标识信息来追踪并限制其请求次数。（[45:11](https://youtu.be/Qa-7iWxDz1A?t=2711)）
%% ytkb:end %%

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- rate limiting 通过为客户端设置单位时间内的请求次数上限（如每段时间100次），超出该上限的请求会被拒绝，需等待一段时间后才能再次发起请求。（[1:54:33](https://youtu.be/oYxTTirKY8M?t=6873)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[http-429-too-many-requests]]
- [[model-gateway]]
- [[request-batching]]
%% ytkb:end %%
