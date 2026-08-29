---
video_id: cbB3QEwWMlA
title: Web Assembly (WASM) in 100 Seconds
source: '[[2020-10-26-web-assembly-wasm-in-100-seconds]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: 9349e396a9312cae39162af03ab27256732e68ce613da6b4625fb9019e32ce08
  schema_version: 1
  model: sonnet
  generated_at: '2026-08-26T18:28:54+00:00'
---

## 一句话总结

[[webassembly|WebAssembly]] 是 2019 年 12 月成为 W3C 官方标准的低层级类汇编语言，它不是要取代 JavaScript，而是作为 C++、Rust、AssemblyScript 等语言的编译目标，让浏览器能以接近原生的性能运行高性能代码。

## 核心内容

### WebAssembly 是什么、解决什么问题

[[webassembly|WebAssembly]]（00:00）包含一种类似汇编语言的低层级语言，既可以用可读的文本格式表示，也能转换成可在所有现代浏览器上运行的二进制格式。它于 2019 年 12 月正式成为 W3C 标准。它的定位很关键：并非用来取代 JavaScript，而是与 JavaScript 协同工作。视频举了 Figma 的例子——外层 UI 用 React.js 构建，内部则运行编译为 WebAssembly 的高性能 C++ 设计引擎，性能接近原生软件。也正因如此，开发者通常不会直接手写 WebAssembly 代码，而是把它当作用 C++、Rust、Python、Go 等语言编写程序的编译目标（compilation target）。

### 两条上手路径：AssemblyScript 与 Emscripten

对于想直接体验 WebAssembly 开发的人，[[assemblyscript|AssemblyScript]]（00:00）是入门的最佳方式之一：它的语法类似 TypeScript，但编译产物是 WebAssembly。用 Node.js 和 npm 就能快速创建一个 AssemblyScript 项目，在 index.ts 文件中编写模块代码。

如果目标是把已有的 C/C++ 代码搬上 Web，[[emscripten|Emscripten]]（00:00）是最流行的构建工具之一，可以将 C 或 C++ 程序编译为 WebAssembly。一个很能说明问题的案例是：Emscripten 曾被用来把拥有 30 年历史的 AutoCAD 代码库移植到网页端。

### 静态类型：WebAssembly 与 JavaScript 的本质差异

与动态解释型的 JavaScript 不同，[[wasm-static-typing|WebAssembly 是静态编译语言]]（00:00），带有严格的类型保证——AssemblyScript 代码中甚至不允许使用 any 类型。这意味着写数字时必须显式指定具体类型，比如 32 位整数或 64 位浮点数。同时,AssemblyScript 不支持动态对象（dynamic object），如果需要键值对结构，得改用强类型的 Map 来实现，而不能像 JS 那样随手写一个对象字面量。

### 编译产物与浏览器中的加载运行

AssemblyScript 代码编译后会生成一个以 .wasm 为扩展名的[[wasm-binary-format|二进制文件]]（00:00），这正是浏览器实际加载执行的内容。在浏览器端运行该 wasm 模块时，可以用 WebAssembly API 的 [[webassembly-instantiatestreaming|instantiateStreaming]] 方法（00:00）直接 fetch 这个二进制文件，并在返回的 promise resolve 之后执行相应的调用逻辑，从而把 wasm 模块无缝集成进网页应用中。

## 值得记住的细节

- [00:00] [[webassembly|WebAssembly]] 于 2019 年 12 月成为官方 W3C 标准。
- [00:00] Emscripten 曾用于将 30 年历史的 AutoCAD 代码库移植到网页端，是 C/C++ 转 WebAssembly 的代表案例。
- [00:00] Figma 采用 React.js（UI）+ WebAssembly 编译的 C++ 设计引擎（性能核心）的混合架构。
- [00:00] AssemblyScript 语法类似 TypeScript，但不支持 any 类型，也不支持动态对象，键值对需用 Map 实现。
- [00:00] AssemblyScript 数字必须显式声明类型，例如 32 位整数或 64 位浮点数。
- [00:00] AssemblyScript 编译产物是 .wasm 二进制文件。
- [00:00] 浏览器中用 WebAssembly.instantiateStreaming 直接 fetch .wasm 文件并在 promise resolve 后执行。
- [00:00] 用 Node.js + npm 即可快速搭建 AssemblyScript 项目。

## 这个视频适合谁 / 可以跳过什么

这是一条 Fireship 风格的 100 秒速览视频，适合完全没接触过 [[webassembly|WebAssembly]]、想在两分钟内建立整体概念（是什么、为什么存在、和 JS 的关系、怎么上手）的开发者。如果你已经用过 [[assemblyscript|AssemblyScript]] 或 [[emscripten|Emscripten]] 做过实际项目，或者已经了解 [[wasm-static-typing|WebAssembly 的静态类型系统]]和[[wasm-binary-format|二进制格式]]，这条视频信息密度较低，内容基本可以跳过，不会有新增知识。
