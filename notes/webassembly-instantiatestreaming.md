---
title: WebAssembly.instantiateStreaming
aliases: []
tags:
- concept
summary: instantiateStreaming 是 WebAssembly API 提供的方法，用于流式获取并实例化 wasm 二进制模块，供浏览器运行。
created: '2026-08-26'
updated: '2026-08-26'
---

# WebAssembly.instantiateStreaming

%% ytkb:def %%
instantiateStreaming 是 WebAssembly API 提供的方法，用于流式获取并实例化 wasm 二进制模块，供浏览器运行。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-webassembly]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:cbB3QEwWMlA %%
### 来自 [[2020-10-26-web-assembly-wasm-in-100-seconds]]
- 在浏览器中运行 wasm 模块时，可以使用 WebAssembly API 的 instantiateStreaming 方法直接 fetch 该二进制文件，并在返回的 promise resolve 后执行相应逻辑。（[00:00](https://youtu.be/cbB3QEwWMlA?t=0)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[wasm-binary-format]]
- [[webassembly]]
%% ytkb:end %%
