---
video_id: 5C_HPTJg5ek
url: https://www.youtube.com/watch?v=5C_HPTJg5ek
title: Rust in 100 Seconds
channel: Fireship
published: '2021-10-12'
duration: 02:29
transcript_origin: subs
tags:
- video
---

# Rust in 100 Seconds

摘要: [[2021-10-12-rust-in-100-seconds-summary|完整摘要]]

## 知识点

- [[borrow-checker-rust]] — Rust 的 borrow checker 会在编译期验证 ownership 与 borrowing 相关规则，从而在保证内存安全的同时保留对性能的完全控制。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[borrowing-rust]] — Borrowing 允许程序的其他部分通过引用（reference）访问某个值，而无需转移其 ownership。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[cargo-package-manager]] — Rust 使用名为 cargo 的包管理器，每个独立的包称为一个 crate。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[crate-rust]] — 在 Rust 生态中，每个通过 cargo 管理的独立包被称为一个 crate。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[garbage-collector]] — 传统高级语言依靠垃圾回收器（garbage collector）自动管理内存但削弱了开发者对内存的控制，而传统底层语言通过 free/allocate 等函数手动管理内存、容易出错。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[heap-memory]] — 可变值（mutable values）或编译期大小未知的对象会被存放在 heap memory 中。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[immutability-default-rust]] — Rust 中变量默认是不可变的，这使得未标记为 mutable 的值可以安全地存放在 stack memory 中，运行时开销更低。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[let-keyword-rust]] — 使用 `let` 关键字声明变量时需指定变量名和类型，且该变量默认不可变、不能被重新赋值。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[mut-keyword-rust]] — 在 `let` 声明前添加 `mut` 关键字可以使变量变为可变（mutable），从而允许修改其值。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[ownership-rust]] — Rust 不使用垃圾回收器，而是通过 ownership 与 borrowing 机制在编译期保证内存安全。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[println-macro-rust]] — 使用 `println!` 宏可以将变量的值打印到标准输出。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[rust-programming-language]] — Rust 适合构建对性能要求极高的系统，如游戏引擎、数据库、操作系统，也是编译到 WebAssembly 的优秀选择。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[rust-standard-library]] — Rust 标准库包含处理 IO、文件系统和并发（concurrency）等功能的内置模块。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[rustc]] — 使用 rustc（Rust 编译器）可以将 Rust 源代码编译成一个内存安全的可执行文件。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[stack-memory]] — 编译期大小已知的不可变值存放在 stack memory 中，性能开销最小。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
- [[webassembly]] — Rust 是将代码编译到 WebAssembly（Wasm）目标时的优秀语言选择。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
