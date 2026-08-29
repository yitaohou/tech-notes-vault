---
title: Context Engineering
aliases: []
tags:
- concept
summary: Anthropic 提出的概念，指构建和管理系统提示词、动态技能、本地配置、自动记忆和丰富引用等复杂上下文生态系统的过程。
created: '2026-08-26'
updated: '2026-08-26'
---

# Context Engineering

%% ytkb:def %%
Anthropic 提出的概念，指构建和管理系统提示词、动态技能、本地配置、自动记忆和丰富引用等复杂上下文生态系统的过程。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-prompt-engineering]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- Anthropic 把构建和管理系统提示词、动态技能、本地配置、自动记忆和丰富引用这个复杂生态系统的过程，称为『上下文工程』（Context Engineering）。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
- 系统提示词虽然被大幅精简，但 Anthropic 并未放弃提示工程，而是再次强调了范围更大的 Context Engineering 概念，且该概念至少从2025年起就被系统性提出，并非新词。（[06:01](https://youtu.be/Lle_EJljIoo?t=361)）
- 提示词只是对 AI 说的一句话，而上下文是 AI 做决策所依赖的全部背景信息，二者范畴不同。（[06:01](https://youtu.be/Lle_EJljIoo?t=361)）
- 新模型生成的代码出现 bug 或跑不起来，很多时候不是模型能力不够，而是给的上下文不对，比如参考资料混乱、项目边界不清、该给的信息没给。（[06:01](https://youtu.be/Lle_EJljIoo?t=361)）
- 随着模型推理能力进化，Prompt Engineering 正在向 Context Engineering 演进，本质上是向传统软件工程思维的回归。（[09:45](https://youtu.be/Lle_EJljIoo?t=585)）
- 好的上下文工程要求工具接口设计得足够自解释，参数命名清晰、类型定义准确。（[10:05](https://youtu.be/Lle_EJljIoo?t=605)）
- 给模型的参考资料应尽量提供高保真的代码和测试用例，而非模糊的文字描述，这比花几个小时抠提示词字眼要有用得多。（[10:15](https://youtu.be/Lle_EJljIoo?t=615)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-5]]
- [[claude-code]]
- [[context-ecosystem-claude-code]]
- [[prompt-engineering]]
- [[rich-context-references]]
- [[thariq-shihipar]]
%% ytkb:end %%
