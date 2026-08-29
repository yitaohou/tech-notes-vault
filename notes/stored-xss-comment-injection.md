---
title: Stored XSS via Comment Injection
aliases: []
tags:
- concept
summary: 攻击者在评论区等用户输入入口提交含恶意脚本的内容，该内容被后端存入数据库，后续其他用户加载评论时脚本会在其浏览器中被执行的存储型 XSS 攻击方式。
created: '2026-08-26'
updated: '2026-08-26'
---

# Stored XSS via Comment Injection

%% ytkb:def %%
攻击者在评论区等用户输入入口提交含恶意脚本的内容，该内容被后端存入数据库，后续其他用户加载评论时脚本会在其浏览器中被执行的存储型 XSS 攻击方式。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-api-gateway-security]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:oYxTTirKY8M %%
### 来自 [[2026-05-26-system-design-explained-apis-databases-caching-cdn]]
- 若 API 未对用户提交的评论内容做过滤就直接存入数据库，攻击者可在评论中植入脚本，之后其他用户加载该评论时，浏览器会在其页面环境中执行这段被注入的恶意 JavaScript，可能用于窃取其他用户的 cookie 或篡改数据库。（[2:00:34](https://youtu.be/oYxTTirKY8M?t=7234)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[csrf-attack]]
- [[xss-attack]]
%% ytkb:end %%
