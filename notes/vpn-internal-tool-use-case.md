---
title: VPN for Internal Tools
aliases: []
tags:
- concept
summary: 把内部管理后台等工具的 API 部署在公司 VPN 内，只有连接了公司 VPN 的员工才能访问的典型使用场景。
created: '2026-08-26'
updated: '2026-08-26'
---

# VPN for Internal Tools

%% ytkb:def %%
把内部管理后台等工具的 API 部署在公司 VPN 内，只有连接了公司 VPN 的员工才能访问的典型使用场景。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 内部 admin 后台的 API 通常只对接入公司 VPN 的员工开放，是 VPN 隔离网络访问的典型应用场景。（[2:00:34](https://youtu.be/oYxTTirKY8M?t=7234)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[vpn-api-access-restriction]]
%% ytkb:end %%
