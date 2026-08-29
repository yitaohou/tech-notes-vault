---
title: Token-Based Usage Limiting
aliases: []
tags:
- concept
summary: 以 token 等类似“货币”的计量单位而非单纯请求次数作为限制维度的用量限制方式，例如 Claude Code、ChatGPT 的每日 token
  额度。
created: '2026-08-26'
updated: '2026-08-26'
---

# Token-Based Usage Limiting

%% ytkb:def %%
以 token 等类似“货币”的计量单位而非单纯请求次数作为限制维度的用量限制方式，例如 Claude Code、ChatGPT 的每日 token 额度。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-coding-agents]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- Claude Code 和 ChatGPT 的每日 token 额度本质上和 rate limiting 是同一种思路，只是把限制的资源单位从请求次数换成了 token，因为这类计算资源成本高昂。（[45:11](https://youtu.be/Qa-7iWxDz1A?t=2711)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-code]]
- [[rate-limiting]]
%% ytkb:end %%
