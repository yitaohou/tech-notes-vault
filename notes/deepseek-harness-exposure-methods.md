---
title: DeepSeek Harness Exposure Methods
aliases: []
tags:
- concept
summary: 使该漏洞可被远程利用的两种典型部署暴露方式：云服务器端口映射直接暴露管理端口，或挂反向代理配域名后暴露整套管理接口。
created: '2026-09-03'
updated: '2026-09-03'
---

# DeepSeek Harness Exposure Methods

%% ytkb:def %%
使该漏洞可被远程利用的两种典型部署暴露方式：云服务器端口映射直接暴露管理端口，或挂反向代理配域名后暴露整套管理接口。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 该漏洞被远程利用的前提是管理接口被暴露到公网，典型方式有两种：一是在云服务器上部署 DeepSeek Harness 并做端口映射、把管理端口直接暴露到公网；二是挂反向代理再配上域名，同样会暴露整套管理接口；这两类部署只要攻击者知道地址就能远程接管。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-loopback-binding-limitation]]
- [[deepseek-harness-unauthenticated-management-api]]
%% ytkb:end %%
