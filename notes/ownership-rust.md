---
title: Ownership (Rust)
aliases: []
tags:
- concept
summary: Ownership 是 Rust 的核心内存管理机制：每个值都有唯一的所有者变量，所有者离开作用域时值占用的内存会被自动释放，无需垃圾回收器。
created: '2026-08-26'
updated: '2026-08-26'
---

# Ownership (Rust)

%% ytkb:def %%
Ownership 是 Rust 的核心内存管理机制：每个值都有唯一的所有者变量，所有者离开作用域时值占用的内存会被自动释放，无需垃圾回收器。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[backend-languages-runtimes]] · [[backend]]
%% ytkb:end %%

## 要点

%% ytkb:video:5C_HPTJg5ek %%
### 来自 [[2021-10-12-rust-in-100-seconds]]
- Rust 不使用垃圾回收器，而是通过 ownership 与 borrowing 机制在编译期保证内存安全。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- 在 Rust 中，每个值都被赋给一个唯一的所有者变量（owner），当该变量离开作用域（scope）时，其占用的内存会自动被释放（drop）。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[borrow-checker-rust]]
- [[borrowing-rust]]
- [[garbage-collector]]
%% ytkb:end %%
