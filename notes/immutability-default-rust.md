---
title: Immutability by Default (Rust)
aliases: []
tags:
- concept
summary: Rust 中变量默认不可变（immutable），需要显式使用 mut 关键字才能修改其值。
created: '2026-08-26'
updated: '2026-08-26'
---

# Immutability by Default (Rust)

%% ytkb:def %%
Rust 中变量默认不可变（immutable），需要显式使用 mut 关键字才能修改其值。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-languages-runtimes]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:5C_HPTJg5ek %%
### 来自 [[2021-10-12-rust-in-100-seconds]]
- Rust 中变量默认是不可变的，这使得未标记为 mutable 的值可以安全地存放在 stack memory 中，运行时开销更低。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[stack-memory]]
%% ytkb:end %%
