---
title: DeepSeek Harness Management Port Exposure Risks
aliases: []
tags:
- concept
summary: 两种常见的部署操作会主动把 DeepSeek Harness 无认证的管理端口暴露到公网，从而制造安全风险。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Management Port Exposure Risks

%% ytkb:def %%
两种常见的部署操作会主动把 DeepSeek Harness 无认证的管理端口暴露到公网，从而制造安全风险。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 把 DeepSeek Harness 部署在云服务器上并做端口映射、将3080端口转发到公网，是导致无认证后台被暴露到公网的常见风险操作之一。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
- 给 DeepSeek Harness 挂一个反向代理并绑定域名、把整套管理接口对外发布，同样会导致无认证的后台直接暴露在公网上。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-management-port-config]]
- [[ssh-tunnel-secure-remote-access]]
%% ytkb:end %%
