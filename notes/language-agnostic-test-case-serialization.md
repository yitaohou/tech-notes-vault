---
title: Language-Agnostic Test Case Serialization
aliases: []
tags:
- concept
summary: 将测试用例输入统一序列化为通用格式（如 JSON），再为每种编程语言提供对应的反序列化器，从而避免为不同语言维护不同的测试用例。
created: '2026-08-26'
updated: '2026-08-26'
---

# Language-Agnostic Test Case Serialization

%% ytkb:def %%
将测试用例输入统一序列化为通用格式（如 JSON），再为每种编程语言提供对应的反序列化器，从而避免为不同语言维护不同的测试用例。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[system-design-code-execution-platform]] · [[system-design]]
%% ytkb:end %%

## 要点

%% ytkb:video:QBHTbtWSECg %%
### 来自 [[2026-03-15-system-design-mock-interview-design-leetcode-ft-ex]]
- 为支持多语言判题（如 online judge 系统），可将测试用例统一序列化（例如用 JSON），每种语言只需实现自己的反序列化逻辑（如 C++ 反序列化成 hashmap，Python 反序列化成 dictionary），核心测试数据本身保持不变。（[45:13](https://youtu.be/QBHTbtWSECg?t=2713)）
%% ytkb:end %%
