---
title: WebAssembly
aliases: []
tags:
- concept
summary: WebAssembly（Wasm）是一种可在浏览器等环境高效运行的低层级字节码格式，常作为高性能语言的编译目标。
created: '2026-08-26'
updated: '2026-08-26'
---

# WebAssembly

%% ytkb:def %%
WebAssembly（Wasm）是一种可在浏览器等环境高效运行的低层级字节码格式，常作为高性能语言的编译目标。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-webassembly]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:5C_HPTJg5ek %%
### 来自 [[2021-10-12-rust-in-100-seconds]]
- Rust 是将代码编译到 WebAssembly（Wasm）目标时的优秀语言选择。（[00:00](https://youtu.be/5C_HPTJg5ek?t=0)）
%% ytkb:end %%

%% ytkb:video:cbB3QEwWMlA %%
### 来自 [[2020-10-26-web-assembly-wasm-in-100-seconds]]
- WebAssembly 于 2019 年 12 月成为官方 W3C 标准。（[00:00](https://youtu.be/cbB3QEwWMlA?t=0)）
- WebAssembly 包含一种类似汇编语言的低层级语言，可以用文本格式表示，再转换为可在所有现代浏览器上运行的二进制格式。（[00:00](https://youtu.be/cbB3QEwWMlA?t=0)）
- 开发者通常不会直接编写 WebAssembly 代码，而是将其作为用 C++、Rust、Python、Go 等其他语言编写的程序的编译目标（compilation target）。（[00:00](https://youtu.be/cbB3QEwWMlA?t=0)）
- WebAssembly 并非用来取代 JavaScript，而是与其协同工作；例如 Figma 用 React.js 构建外层 UI，内部则运行编译为 WebAssembly 的高性能 C++ 设计引擎，性能接近原生软件。（[00:00](https://youtu.be/cbB3QEwWMlA?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[assemblyscript]]
- [[emscripten]]
- [[rust-programming-language]]
- [[wasm-binary-format]]
%% ytkb:end %%
