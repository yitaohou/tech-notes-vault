---
title: Stable Vendor Chunk with Long max-age
aliases: []
tags:
- concept
summary: 把很少变动的稳定依赖（如 React、ReactDOM）打包成独立的长期稳定 chunk，并设置较长的 max-age（如7天），以避免用户反复重新下载这部分代码。
created: '2026-08-26'
updated: '2026-08-26'
---

# Stable Vendor Chunk with Long max-age

%% ytkb:def %%
把很少变动的稳定依赖（如 React、ReactDOM）打包成独立的长期稳定 chunk，并设置较长的 max-age（如7天），以避免用户反复重新下载这部分代码。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-architecture]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- 像 React、ReactDOM 这类几乎每年都不会变的稳定第三方库，应该被打包进单独的 chunk 文件，并设置较长的 max-age（例如7天），减少客户端重复下载。（[42:09](https://youtu.be/AMerB8XjfZ0?t=2529)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[frontend-bundle-splitting]]
- [[selective-caching-policy-frontend]]
%% ytkb:end %%
