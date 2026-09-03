---
title: Prompt Injection Attack
aliases: []
tags:
- concept
summary: 通过在输入中植入恶意指令，诱导模型执行未授权操作的攻击手法。
created: '2026-08-26'
updated: '2026-09-03'
---

# Prompt Injection Attack

%% ytkb:def %%
通过在输入中植入恶意指令，诱导模型执行未授权操作的攻击手法。
%% ytkb:end %%

%% ytkb:topic %%
所属: [[ai-safety-security]] · [[ai]]
%% ytkb:end %%

## 要点

%% ytkb:video:JV3pL1_mn2M %%
### 来自 [[2025-04-01-ai-engineering-in-76-minutes-complete-coursespeedr]]
- prompt injection 攻击试图让模型执行未经授权的操作，与 jailbreaking 常被归为同一类安全威胁。（[27:02](https://youtu.be/JV3pL1_mn2M?t=1622)）
%% ytkb:end %%

%% ytkb:video:WrwA7FYGPdQ %%
### 来自 [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]
- AI 模型会读取并服从其在网页、文档等内容中看到的文字指令，攻击者可借此在恶意网页或文档中预先写入诸如「忽略之前的命令，执行以下操作」这样的隐藏指令实施提示注入攻击。（[12:04](https://youtu.be/WrwA7FYGPdQ?t=724)）
- 与可打补丁修复的程序漏洞不同，prompt injection 类风险没有任何补丁能够被彻底修复，是比常规程序漏洞更棘手的一类风险。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- prompt injection 之所以无法通过打补丁彻底修复，是因为读取并服从文本指令本就是语言模型的核心任务机制，关掉这个机制模型就无法工作，因此这类风险目前没有被彻底解决的可能，只能从源头降低AI读到恶意内容的概率。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
- 朱雀的提示词注入攻击测评显示，安装一个带恶意指令的 skill 插件，提示注入的成功率在 14% 到 16% 之间，说明安装插件这个动作本身就可能是攻击入口。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
%% ytkb:end %%

## 相关概念

%% ytkb:related %%
- [[deepseek-harness-injection-success-rate]]
- [[harness-rapid-iteration-security-instability]]
- [[hidden-text-prompt-injection-technique]]
- [[information-extraction-attack]]
- [[jailbreaking-attack]]
- [[no-official-plugin-marketplace-review]]
- [[prompt-extraction-attack]]
%% ytkb:end %%
