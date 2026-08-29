---
title: DNS Domain-to-IP Resolution
aliases: []
tags:
- concept
summary: DNS（domain name system）是把域名映射到服务器 IP 地址的服务，客户端需先查询 DNS 才能知道请求应发往哪里。
created: '2026-08-26'
updated: '2026-08-26'
---

# DNS Domain-to-IP Resolution

%% ytkb:def %%
DNS（domain name system）是把域名映射到服务器 IP 地址的服务，客户端需先查询 DNS 才能知道请求应发往哪里。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-networking]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 当用户在浏览器或 App 中访问类似 app.demo.com 的域名时，设备会先向 DNS 查询，DNS 返回该域名对应的服务器 IP 地址后，客户端才能据此向服务器发送 HTTP 请求。（[03:00](https://youtu.be/oYxTTirKY8M?t=180)）
%% ytkb:end %%
