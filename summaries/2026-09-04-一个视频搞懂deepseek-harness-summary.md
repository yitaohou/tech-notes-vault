---
video_id: buYQ-_V2Wv0
title: 一个视频搞懂DeepSeek Harness！
source: '[[2026-09-04-一个视频搞懂deepseek-harness]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: 493d69461d4feb85cfb7bb27e80808e52227af8d3959a55cf72e21c68ee7de0e
  schema_version: 1
  model: sonnet
  generated_at: '2026-09-04T20:52:25+00:00'
---

## 一句话总结

DeepSeek 开源了自己的 Agent Harness——一个默认几乎空白、靠插件拼装出全部功能的框架，两天涨 10 万 star；它不仅解释了 V4 Pro 跑分虚高的争议根源，还通过底层的 Cordis 系统展示了一种可能重塑 AI 时代应用生态的"可组合性"新思路。

## 核心内容

### 为什么 DeepSeek 要自己做 Harness

[[agent-model-harness-formula|Agent 能力可以拆解为"模型 + Harness"]]（00:00），类比成"模型是发动机，Harness 是车架"——同一个模型换不同车架表现天差地别，比如 Claude 模型接 Claude Code 效果拔群，接 Codex 就掉链子。[[deepseek-harness-motivation|DeepSeek 正是意识到用别人家 Harness 会有话语权不对称、能力发挥受限的问题]]（00:00），于是决定自己开源一个 Harness，让模型能力充分释放。这一举动发生在 [[ai-office-software-competition-2026|2026 年下半年 AI 办公软件混战正酣]]（00:00）的背景下——市面上各家都在追求低门槛高覆盖，DeepSeek Harness 却反其道而行，[[deepseek-harness-empty-default-install|默认安装后只有一个空荡荡的本地网页]]（00:00），技能市场、文件上传等基础功能全靠用户照说明文档自行拼装。即便如此，它依然创下了 [[deepseek-harness-github-star-growth|开源两天 10 万星、GitHub 历史增速前三]]（00:00）的成绩，力压 OpenClaw。

支撑这套空壳的是庞大的插件生态：[[deepseek-harness-plugin-count|前端 57 个插件 + 后端 78 个插件]]（00:00），从滑动变阻器到记忆调度模式，几乎所有功能都能通过插件实现或替换。

### V4 Pro 跑分争议的真相：四种模式与"机械模式"

[[deepseek-v4-pro-benchmark-controversy|V4 Pro 发布时官方跑分逼近 Claude Opus 5，但实际使用体验却经常不如参数更小的 V4 Flash]]（00:00），这个长期存在的谜团在 Harness 开源后被揭开。DeepSeek Harness 自带 [[deepseek-harness-modes|四种运行模式]]（00:00），其中 [[deepseek-harness-mechanical-mode|极简模式（官方定位为基准测试专用）只保留终端和文件编辑器两个工具]]（00:00），没有任务规划、没有联网搜索、连上下文压缩都没有。原因在于：[[deepseek-v4-pro-mechanical-mode-post-training|V4 Pro 针对极简模式做了专门后训练]]（00:00），一看到只有两个工具就会进入高效状态；但一旦把各种工具全部塞给它，反而会犯迷糊、办事拖泥带水。基于这个发现，有开发者做出了 [[liangshen-mode-plugin|"量神模式"双阶段插件]]（00:00），先用极简模式激发 V4 Pro 的高水平思维链，再切回正常工作，从而规避工具过多导致的性能下降。

与之相印证的是，[[deepseek-harness-batch-script-mode|PTC 批处理模式]]（03:01）把多个工具调用一次性写进脚本执行，而不是每用一次工具就停下思考一次，这样能减少模型的思考步骤，使其不容易从高水平思维链退化回逐步试探的低效模式——本质上也是在维持模型的"高效工作状态"。

### 插件生态实测：从权限管理到日常效率工具

DeepSeek Harness 官方模式中，[[deepseek-harness-creative-mode|创造模式可玩性最高]]（03:01），允许用户直接编写新插件。而权限管理是绕不开的痛点：[[deepseek-harness-permission-tiers|只读/工作区可写两档权限操作繁琐，完全访问档虽自由但已出现文件被一键删光的真实案例]]（03:01）。为此 [[dsh-approval-gate-plugin|DSH-Approval-Gate 插件]]（03:01）让智能体先自查风险，简单命令直接放行、危险命令转人工审批，用久后还会根据用户习惯自动改进放行规则，历史申请也可在新增标签页查看。

其他实用插件还包括：应对反爬虫的 [[dsh-ego-browser-plugin|DSH-EGO Browser]]（03:01，模拟人类操作浏览器，过程可在侧栏观察）；扩大搜索范围或为非官方模型补齐联网能力的 [[mod-search-plugin|MOD Search]]（03:01）；一次集齐侧边栏、插件市场、远程控制、量神模式的整合包 [[dsh-web-ui-plugin|DSH-Web UI]]（03:01）；把执行任务外包给已订阅的 Codex/Claude Code、让 DeepSeek 专注规划的 [[dsh-sub-agent-codex-plugin|DSH Sub-Agent Codex]]（03:01，理由是执行到位比规划模型聪明更重要）。

省钱方面，[[deepseek-peak-off-peak-pricing|DeepSeek 工作日峰谷计价，高价时段（"梁文峰时段"）是低价时段（"梁文股时段"）的两倍]]（03:01），过去一天一块钱够用的时代已经过去；对应有 [[peak-price-reminder-plugin|峰谷计价浮窗提醒插件]]（03:01）和 [[thinking-intensity-slider-plugin|可调节思考强度挡位的滑动变速器插件（简单任务调低以省额度）]]（03:01）。此外还有纯粹好玩/实用的副产品：[[stock-market-plugin|股票大盘插件]]（03:01）可直接在界面盯盘，[[gomoku-dual-ai-plugin|五子棋类插件]]（03:01）能让用户在新标签页观摩两个 AI 对战。

### 底层野心：Cordis 与"可组合性"

支撑这一切插件能协同运行的，是名为 [[cordis-plugin-runtime-foundation|Cordis 的底层基座系统]]（06:02）。DeepSeek 发表的 [[deepseek-cordis-spacetime-paper|Cordis 时空论文]]（06:02）从数学上证明该系统同时具备 [[temporal-composability|时间可组合性]]（06:02）与 [[spatial-composability|空间可组合性]]（06:02）——这直接对照了 [[traditional-software-composability-weakness|传统软件体系可组合性差的痛点]]（06:02）：删除游戏后存档配置依然残留注册表（时间不可撤销）、联机工具/MOD 管理器/作弊器依然留在系统里（空间不可撤销），这也是系统清理工具长盛不衰的原因。若无良好的可组合性机制，[[agent-dynamic-plugin-garbage-accumulation|Agent 动态创建/升级/删改工具的过程会导致垃圾文件堆积，旧插件残留还可能让新插件跑不起来]]（06:02）。

作者用 [[lego-modularity-analogy-harness|乐高 1958 年"拼装原件"专利]]（06:02）类比：正是凸钉与套管的标准接插结构，让乐高从零件有限发展成能拼出任意形态的无限组合系统，DeepSeek Harness 的可组合性架构有望走同样的路。结合 [[post-web-coding-app-fragmentation|Vibe Coding 让开发成本骤降、软件越写越多越碎（甚至一个 App 只服务几个人用几次就丢）]]（06:02）的趋势，作者提出 [[harness-as-app-container-vision|DeepSeek Harness 有潜力成为承载这种散碎应用生态的新容器，即"AI 时代的应用市场"]]（06:02）——模型、工具、技能、界面都可在同一基座上自由替换组合，形态可以干净切换。界面本身也是插件的例证是 [[harness-ui-reskin-plugin|Galview 插件可把默认输入框界面改造成恋爱游戏风格]]（06:02）。

不过这个愿景也有现实压力：[[harness-core-update-breaking-plugins|DeepSeek 官方明确表示核心代码还会有破坏性升级，一更新插件红一大片会是常态，如何管理已近 13000 个插件是待解决问题]]（06:02）。

### 一个题外的模型能力对比

作者顺带做了个小实验：[[gameplay-based-model-capability-comparison|让 V4 Flash、V4 Pro 与 GLM5.3 Flash 玩同一款连线游戏]]（06:02），结果 V4 Flash 和 V4 Pro 眼睁睁看着对手连成三四子也不主动防守反击，而 GLM5.3 Flash 能有来有回甚至布出双重杀阵获胜，体现出模型能力上的明显差距。

## 值得记住的细节

- DeepSeek Harness 开源两天内涨 10 万 GitHub star，速度居历史前三，超过 OpenClaw（00:00）
- 前端 57 个插件 + 后端 78 个插件构成整套系统（00:00）
- 极简模式只有终端+文件编辑器两个工具，是官方定位的基准测试专用模式（00:00）
- V4 Pro 针对极简模式做过专门后训练，工具一多反而表现下降，这是其跑分与实际体验落差的关键原因（00:00）
- "量神模式"插件通过先用极简模式激发思维链再正常工作来规避此问题（00:00）
- PTC 批处理模式把多个工具调用写进一个脚本一次执行，减少思考步骤、省 token（03:01）
- 完全访问权限档已有真实案例导致文件被一键删光，需谨慎；DSH-Approval-Gate 插件可在只读与完全访问间取得平衡，且会随使用习惯自动改进放行规则（03:01）
- DeepSeek 工作日峰谷计价：高价时段（"梁文峰时段"）API 价格是低价时段（"梁文股时段"）的两倍（03:01）
- Cordis 论文从数学上证明了插件系统同时具备时间可组合性和空间可组合性（06:02）
- 乐高 1958 年申请的"一种玩具拼装原件"专利确立了凸钉+套管的接插结构，是作者类比 Harness 未来发展的参照系（06:02）
- 官方已明确未来核心代码会有破坏性升级，插件生态已近 13000 个，管理难度是现实待解问题（06:02）
- 小实验：V4 Flash/V4 Pro 在连线游戏中不会主动防守反击，GLM5.3 Flash 能布双重杀阵获胜（06:02）

## 这个视频适合谁 / 可以跳过什么

适合：想了解 DeepSeek 生态最新动向、关心 Agent Harness 架构设计、对"可组合性/插件化"技术理念感兴趣、以及日常使用 DeepSeek API 想找省钱和效率插件的开发者与重度用户。

可以跳过：如果只关心如何快速上手使用 DeepSeek Harness 而不关心底层原理，可跳过 06:02 之后关于 Cordis 论文、乐高类比和应用生态愿景的理论探讨部分；如果不使用 DeepSeek 模型，V4 Pro 跑分争议部分（00:00 段）也可跳过。
