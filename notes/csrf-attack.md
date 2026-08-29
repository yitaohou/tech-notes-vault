---
title: CSRF (Cross-Site Request Forgery)
aliases: []
tags:
- concept
summary: 跨站请求伪造，指诱导已登录用户的浏览器在其不知情的情况下向目标 API 发起非本意的请求。
created: '2026-08-26'
updated: '2026-08-26'
---

# CSRF (Cross-Site Request Forgery)

%% ytkb:def %%
跨站请求伪造，指诱导已登录用户的浏览器在其不知情的情况下向目标 API 发起非本意的请求。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-security]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 若银行系统仅依赖 session cookie 做身份验证而缺乏额外校验，恶意网站可以利用用户浏览器中已有的 cookie 冒充其身份，偷偷提交转账等请求。（[2:00:34](https://youtu.be/oYxTTirKY8M?t=7234)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[csrf-token-defense]]
%% ytkb:end %%
