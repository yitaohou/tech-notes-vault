---
title: Premature Optimization Caution
aliases: []
tags:
- concept
summary: 系统设计中应避免过早引入性能优化手段（如 caching），以防造成不必要的过度工程化，应等到规模问题真正出现后再着手优化。
created: '2026-08-26'
updated: '2026-08-26'
---

# Premature Optimization Caution

%% ytkb:def %%
系统设计中应避免过早引入性能优化手段（如 caching），以防造成不必要的过度工程化，应等到规模问题真正出现后再着手优化。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-architecture-fundamentals]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:Qa-7iWxDz1A %%
### 来自 [[2026-06-08-fundamentals-of-backend-architecture---how-to-desi]]
- caching、CDN、rate limiting 这类性能优化应放在系统设计讨论的最后阶段引入，避免 premature optimization 导致过度工程化（overengineering）。（[36:09](https://youtu.be/Qa-7iWxDz1A?t=2169)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[caching-motivation-repeated-access]]
%% ytkb:end %%
