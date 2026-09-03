---
title: Plaintext Injection Testing Blindspot
aliases: []
tags:
- concept
summary: 指仅用纯文本形式测试prompt injection攻击会遗漏真实攻击行为，因为攻击者可将指令换到隐蔽位置从而绕过防御，这一发现来自安全测评论文原文。
created: '2026-09-03'
updated: '2026-09-03'
---

# Plaintext Injection Testing Blindspot

%% ytkb:def %%
指仅用纯文本形式测试prompt injection攻击会遗漏真实攻击行为，因为攻击者可将指令换到隐蔽位置从而绕过防御，这一发现来自安全测评论文原文。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- 测评论文原文指出「只测纯文本会漏掉真实的攻击行为」，意味着即便纯文本注入测试全部被防住，换个藏身位置攻击仍可能成功。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[hidden-injection-payload-location]]
%% ytkb:end %%
