---
title: Borrowing (Rust)
aliases: []
tags:
- concept
summary: Borrowing 是 Rust 中在不获取所有权的前提下访问某个值的引用的机制。
created: '2026-08-26'
updated: '2026-08-26'
---

# Borrowing (Rust)

%% ytkb:def %%
Borrowing 是 Rust 中在不获取所有权的前提下访问某个值的引用的机制。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-languages-runtimes]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:5C_HPTJg5ek %%
### 来自 [[2021-10-12-rust-in-100-seconds]]
- Borrowing 允许程序的其他部分通过引用（reference）访问某个值，而无需转移其 ownership。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- 在 Rust 代码中，通过在变量名前加上 `&`（ampersand）前缀，可以借用（borrow）该变量所在内存位置的引用。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[borrow-checker-rust]]
- [[ownership-rust]]
%% ytkb:end %%
