---
title: Context Dilution
aliases: []
tags:
- concept
summary: 提示词或上下文中包含过多无关内容，会稀释模型注意力、降低其表现的现象。
created: '2026-08-26'
updated: '2026-08-26'
---

# Context Dilution

%% ytkb:def %%
提示词或上下文中包含过多无关内容，会稀释模型注意力、降低其表现的现象。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-rag]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- Anthropic 工程师发现，太多无关上下文会稀释模型注意力，过去『保姆式』的提示词反而成了限制模型发挥的枷锁。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
%% ytkb:end %%

%% ytkb:video:hA_XnzB1Ef8 %%
### 来自 [[2026-07-07-3-frontend-skills-ai-cant-replace-become-ai-proof]]
- 把整个代码库都丢给 AI 去查找已实现的可复用功能，会因为上下文过大而稀释注意力，让模型进入表现下降的「dumb zone」，最终结果反而更差。（[09:03](https://youtu.be/hA_XnzB1Ef8?t=543)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[context-rot]]
- [[context-window-limits-large-models]]
- [[hardcoded-prompt-rules-limitation]]
- [[system-prompt-reduction-claude-code]]
%% ytkb:end %%
