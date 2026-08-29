---
title: AI Hardcoding Values Instead of Design Tokens
aliases: []
tags:
- concept
summary: AI 模型倾向于把具体数值（颜色、像素）硬编码进代码，而不是复用已有的 design token 或框架提供的原子样式类。
created: '2026-08-26'
updated: '2026-08-26'
---

# AI Hardcoding Values Instead of Design Tokens

%% ytkb:def %%
AI 模型倾向于把具体数值（颜色、像素）硬编码进代码，而不是复用已有的 design token 或框架提供的原子样式类。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[frontend-ai-coding-assistants]] · [[frontend]]
%% ytkb:end %%

## 要点

%% ytkb:video:AMerB8XjfZ0 %%
### 来自 [[2026-06-30-top-15-frontend-interview-questions-for-2026-wa-se]]
- AI 模型即便使用了 Tailwind，也常常不用 font-xs 这类原子 CSS class，而是直接写死 font-11px 这样的硬编码数值。（[03:00](https://youtu.be/AMerB8XjfZ0?t=180)）
%% ytkb:end %%

%% ytkb:video:hA_XnzB1Ef8 %%
### 来自 [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof]]
- 即使项目已经配置好设计系统（如 Tailwind），AI 在还原用户提供的截图时仍可能写死具体数值（如 text-28px），而不是复用已有的预定义原子样式类。（[06:02](https://youtu.be/hA_XnzB1Ef8?t=362)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[ai-prompt-to-ui-overoptimization]]
- [[ai-target-hyperoptimization-root-cause]]
- [[atomic-css]]
- [[relative-css-units-ai-constraint]]
- [[relative-sizing-units]]
%% ytkb:end %%
