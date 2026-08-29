---
title: API Gateway
aliases: []
tags:
- concept
summary: 位于客户端与内部服务之间的组件，负责接收请求、分析后转发到正确的后端服务。
created: '2026-08-26'
updated: '2026-08-26'
---

# API Gateway

%% ytkb:def %%
位于客户端与内部服务之间的组件，负责接收请求、分析后转发到正确的后端服务。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- API Gateway 接收客户端请求，对其进行分析后转发到正确的后端服务。（[21:05](https://youtu.be/Qa-7iWxDz1A?t=1265)）
%% ytkb:end %%

%% ytkb:video:KuClyhvSzXk %%
### 来自 [[2026-06-18-frontend-system-design-explained-w-senior-engineer]]
- 如果每次都要在前端和后端两侧分别重复实现 caching、认证、限流等 edge functions，会造成大量重复劳动，这正是引入 API gateway 集中处理这些功能的动机。（[06:02](https://youtu.be/KuClyhvSzXk?t=362)）
- 引入 API gateway 后，客户端只需实现一次 HTTPS handshake、caching、rate limiting 等 edge function，后端服务无需关心这些通用逻辑，只需专注自身业务。（[09:03](https://youtu.be/KuClyhvSzXk?t=543)）
%% ytkb:end %%

%% ytkb:video:CyLYY_xb5bQ %%
### 来自 [[2025-08-25-you-can-learn-ai-agent-system-design-in-19-min-rag]]
- 在 AI 客服 agent 系统中，gateway 需要处理身份认证（如 single sign-on）、PII 隐私保护、rate limiting 以及请求去重检查等前置校验工作。（[06:00](https://youtu.be/CyLYY_xb5bQ?t=360)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[api-edge-functions]]
- [[api-gateway-https-http-boundary]]
- [[auth-gate-before-processing]]
- [[gateway-single-entry-point]]
- [[rate-limiting]]
- [[vpc-private-network-isolation]]
%% ytkb:end %%
