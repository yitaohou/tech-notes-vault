---
title: WebAssembly 静态类型系统
aliases: []
tags:
- concept
summary: WebAssembly 及其编译源语言（如 AssemblyScript）采用静态类型系统，具有严格的类型保证，区别于 JavaScript 的动态类型。
created: '2026-08-26'
updated: '2026-08-26'
---

# WebAssembly 静态类型系统

%% ytkb:def %%
WebAssembly 及其编译源语言（如 AssemblyScript）采用静态类型系统，具有严格的类型保证，区别于 JavaScript 的动态类型。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-webassembly]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:cbB3QEwWMlA %%
### 来自 [[2020-10-26-web-assembly-wasm-in-100-seconds]]
- 与动态解释型的 JavaScript 不同，WebAssembly 是静态编译语言，具有严格的类型保证，例如 AssemblyScript 代码中不能使用 any 类型。（[00:00](https://youtu.be/cbB3QEwWMlA?t=0)）
- 在 AssemblyScript 中处理数字时必须显式指定具体类型，例如 32 位整数（32-bit integer）或 64 位浮点数（64-bit floating point）。（[00:00](https://youtu.be/cbB3QEwWMlA?t=0)）
- AssemblyScript 不支持动态对象（dynamic object），需要使用 Map 来实现键值对的强类型化。（[00:00](https://youtu.be/cbB3QEwWMlA?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[assemblyscript]]
- [[webassembly]]
%% ytkb:end %%
