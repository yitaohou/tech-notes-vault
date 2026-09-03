---
title: Hardcoded Prompt Rules Limitation
aliases:
- Prompt Debt
tags:
- concept
summary: 随着模型能力增强，早期为约束模型行为而写的硬性提示词规则可能反而限制模型自身判断力的现象。
created: '2026-08-26'
updated: '2026-09-03'
---

# Hardcoded Prompt Rules Limitation

%% ytkb:def %%
随着模型能力增强，早期为约束模型行为而写的硬性提示词规则可能反而限制模型自身判断力的现象。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-prompt-engineering]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:Lle_EJljIoo %%
### 来自 [[2026-07-26-删掉80提示词后claude-5反而变强了anthropic官方的做减法哲学]]
- 模型能力变强以后，旧时代为约束其行为而写的硬性提示词规则可能开始限制模型自身的判断。（[00:00](https://youtu.be/Lle_EJljIoo?t=0)）
%% ytkb:end %%

%% ytkb:video:Z-4AsgTYv2c %%
### 来自 [[2026-09-02-claude-code-之父建議每六個月刪光你的-claudemd]]
- 以前 Agent 读取文件不可靠时写的绕路流程、漏格式时加的检查规则，在工具和模型都变强后依然留在提示词里，反而变成拖慢模型的阻力。（[00:00](https://youtu.be/Z-4AsgTYv2c?t=0)）
- 提示词负债的累积过程类似公司 SOP 不断增补：员工每次出错就多加一道签核或检查流程，几年后即使换了能力更强的新人，寄一封信仍要经过层层历史遗留的关卡。（[00:00](https://youtu.be/Z-4AsgTYv2c?t=0)）
- 作者的影片制作 skill 因为一年来每次模型犯错就多加几行规则，最终膨胀到三百多行，甚至包含用文字画的九步流程图并强制规定一步都不准跳，是典型的 prompt debt 案例。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[claude-code-harness-refresh-on-model-release]]
- [[claude-skills]]
- [[system-prompt-reduction-claude-code]]
- [[unhobbling]]
- [[verbose-prompt-paradigm]]
%% ytkb:end %%
