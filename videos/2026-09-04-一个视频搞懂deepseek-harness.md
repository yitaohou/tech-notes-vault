---
video_id: buYQ-_V2Wv0
url: https://www.youtube.com/watch?v=buYQ-_V2Wv0
title: 一个视频搞懂DeepSeek Harness！
channel: 林亦LYi
published: '2026-09-04'
duration: 09:36
transcript_origin: whisper
tags:
- video
---

# 一个视频搞懂DeepSeek Harness！

摘要: [[2026-09-04-一个视频搞懂deepseek-harness-summary|完整摘要]]

## 知识点

- [[agent-dynamic-plugin-garbage-accumulation]] — AI智能体在运行过程中会不断动态创建、升级、删改各种小工具，若缺乏良好的可组合性机制，会导致大量垃圾文件堆积在电脑里，且旧插件的残留还可能导致新插件跑不起来。（[06:02](https://youtu.be/buYQ-_V2Wv0?t=362)）
- [[agent-model-harness-formula]] — 该公式可以类比为「模型是发动机，Harness是车架」；同一个模型接不同的 Harness 表现会有明显差异，例如 Claude 模型接 Claude Code 效果拔群，接 Codex 能力就掉下来了。（[00:00](https://youtu.be/buYQ-_V2Wv0?t=0)）
- [[ai-office-software-competition-2026]] — 2026年下半年AI办公软件竞争激烈，Workbody、豆包工作台等各类Work类产品广告随处可见，各方追逐低门槛高覆盖，而DeepSeek Harness反其道而行，采用近乎空白、需自行拼装的插件化架构。（[00:00](https://youtu.be/buYQ-_V2Wv0?t=0)）
- [[cordis-plugin-runtime-foundation]] — DeepSeek Harness之所以能运行数量庞大、种类各异的插件，依赖于一个名为Cordis的底层基座系统。（[06:02](https://youtu.be/buYQ-_V2Wv0?t=362)）
- [[deepseek-cordis-spacetime-paper]] — 该论文从理论上证明了Cordis插件系统同时具备时间可组合性（temporal composability）和空间可组合性（spatial composability），且这一证明是数学上完美的。（[06:02](https://youtu.be/buYQ-_V2Wv0?t=362)）
- [[deepseek-harness-batch-script-mode]] — PTC 模式下模型会把要用到的多个工具调用一次性写进一个脚本执行，而不是每用一次工具就停下来思考一次，从而更省时间和 token。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[deepseek-harness-creative-mode]] — 在 DeepSeek Harness 官方提供的模式中，创造模式可玩性最高，允许用户直接给 DeepSeek Harness 编写新插件。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[deepseek-harness-empty-default-install]] — DeepSeek Harness 默认安装后只有一个空荡荡的本地网页，技能市场、文件上传等基础功能一概没有，用户需要根据说明文档自行拼装组装出完整功能。（[00:00](https://youtu.be/buYQ-_V2Wv0?t=0)）
- [[deepseek-harness-github-star-growth]] — DeepSeek Harness 开源两天内收获10万星，增长速度位居GitHub历史前三，力压老前辈OpenClaw。（[00:00](https://youtu.be/buYQ-_V2Wv0?t=0)）
- [[deepseek-harness-mechanical-mode]] — 极简模式只保留了运行终端和文件编辑器两个工具，没有任务规划、没有联网搜索，连上下文压缩都没有，官方给它的定位是基准测试专用模式，用来衡量模型性能。（[00:00](https://youtu.be/buYQ-_V2Wv0?t=0)）
- [[deepseek-harness-modes]] — DeepSeek Harness 安装好之后自带四种运行模式，大部分任务用默认的标准模式就够了。（[00:00](https://youtu.be/buYQ-_V2Wv0?t=0)）
- [[deepseek-harness-motivation]] — DeepSeek 意识到大模型接别人家的 Harness 会存在能力发挥受限的话语权不对称问题，因此选择自己开源一个 Harness，让 DeepSeek 模型的能力充分释放。（[00:00](https://youtu.be/buYQ-_V2Wv0?t=0)）
- [[deepseek-harness-permission-tiers]] — 只读和工作区可写这两档权限下，即使只是读取一个文件也需要用户手动停下确认，使用体验较为繁琐；而完全访问档虽然自由，但网上已出现因权限过大导致文件被一键删光的真实受害案例。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[deepseek-harness-plugin-count]] — DeepSeek Harness 的前端界面由 57 个插件组成，后端看不见的智能体部分由 78 个插件组成，滑动变阻器、蓝色大肥鱼等复杂功能甚至记忆调度模式都可以通过插件系统实现或替换。（[00:00](https://youtu.be/buYQ-_V2Wv0?t=0)）
- [[deepseek-peak-off-peak-pricing]] — DeepSeek 在工作日实行峰谷计价，官方所称的高价时段（俗称「梁文峰时段」）API 价格是低价时段（俗称「梁文股时段」）的两倍，过去那种一天只花一块钱就够用的时代已经过去。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[deepseek-v4-pro-benchmark-controversy]] — DeepSeek V4 Pro发布时官方跑分直逼最强模型Claude Opus 5，但大家实际使用后发现不是那么回事，有时V4 Pro的表现甚至不如参数更小的V4 Flash模型。（[00:00](https://youtu.be/buYQ-_V2Wv0?t=0)）
- [[deepseek-v4-pro-mechanical-mode-post-training]] — DeepSeek Harness发布后揭示了V4 Pro跑分虚高争议的原因：V4 Pro针对极简模式做了专门后训练，一看到只有终端和文件编辑两个工具就会进入高效工作状态，但如果一上来把各种工具全部塞给它，V4 Pro反而会犯迷糊、办事拖泥带水。（[00:00](https://youtu.be/buYQ-_V2Wv0?t=0)）
- [[dsh-approval-gate-plugin]] — 安装 DSH-Approval-Gate 插件后，智能体在执行命令前会先自查风险：简单无害的命令直接放行，疑似危险的命令则转为人工审批，从而在只读/完全访问两个极端之间取得平衡。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[dsh-ego-browser-plugin]] — 安装 DSH-EGO Browser 插件后，智能体能够以模拟人类手动操作浏览器的方式读取所需网页信息，用于应对经常触发网站反爬虫机制的问题，且其具体操作执行过程可以在侧栏中直接观察到。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[dsh-sub-agent-codex-plugin]] — 如果用户已有 Codex 或 Claude Code 的订阅，可安装 DSH Sub-Agent Codex 这类插件，让 DeepSeek 负责制定计划、再调用 Codex 作为子智能体去执行具体任务，因为执行是否到位比负责规划的模型是否聪明更重要。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[dsh-web-ui-plugin]] — 安装 DSH-Web UI 整合包插件后，相当于一次性集齐侧边栏、插件市场、远程控制和量神模式等常用功能，能让整体使用体验一步到位过半。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[gameplay-based-model-capability-comparison]] — 作者让V4 Flash、V4 Pro与GLM5.3 Flash分别玩同一款连线游戏，发现V4 Flash和V4 Pro眼睁睁看着对手连成三四子也不会主动防守或反击，而GLM5.3 Flash能有来有回、甚至布出双重杀阵直接获胜，体现出模型能力的明显差距。（[06:02](https://youtu.be/buYQ-_V2Wv0?t=362)）
- [[gomoku-dual-ai-plugin]] — 安装该五子棋类插件后，对话框旁会多出一个新标签页，用户可以在其中直接观摩两个 AI 之间的互动过程。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[harness-as-app-container-vision]] — 作者认为DeepSeek Harness在同一套基座之上，模型、工具、技能、界面都可以自由替换组合出各式各样的应用，且应用之间能干净利落地切换形态，这使其有潜力成为承载AI时代散碎应用生态的新容器，即DeepSeek所设想的「AI时代的应用市场」。（[06:02](https://youtu.be/buYQ-_V2Wv0?t=362)）
- [[harness-core-update-breaking-plugins]] — DeepSeek官方明确表示接下来Harness还会有破坏性升级，核心代码一更新、插件红掉一大片会是常态，如何管理已接近13000个的插件成为待解决的现实问题。（[06:02](https://youtu.be/buYQ-_V2Wv0?t=362)）
- [[harness-ui-reskin-plugin]] — 通过安装Galview这类插件，可以把DeepSeek Harness默认的AI输入框界面彻底改造成恋爱游戏风格的界面，说明界面本身也是可替换的插件。（[06:02](https://youtu.be/buYQ-_V2Wv0?t=362)）
- [[lego-modularity-analogy-harness]] — 1958年乐高集团申请的「一种玩具拼装原件」专利确定了积木凸钉与套管的接插结构，使乐高从早期种类有限的零件发展成今天能拼出任意形态的无限组合系统，作者以此类比展望DeepSeek Harness的发展方向。（[06:02](https://youtu.be/buYQ-_V2Wv0?t=362)）
- [[liangshen-mode-plugin]] — 有开发者做了一个叫「量神模式」的双阶段插件，安装后插件会先用极简模式激发出V4 Pro的高水平工作思维链，以此规避V4 Pro在工具过多时表现下降的问题。（[00:00](https://youtu.be/buYQ-_V2Wv0?t=0)）
- [[mod-search-plugin]] — 安装 MOD Search 插件可以让智能体接入国内外多种搜索引擎以获得更广的搜索范围；若使用的是非官方模型、原本缺失联网搜索能力，该插件还能直接补足这项功能。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[peak-price-reminder-plugin]] — 可以在 DeepSeek Harness 插件市场中搜索峰谷计价相关关键词，安装对应的浮窗提醒插件，帮助用户判断当前是否处于高价时段以便节省额度使用。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[post-web-coding-app-fragmentation]] — 作者认为Vibe Coding兴起后，AI会把开发成本压得很低，软件会越写越多、越写越碎，甚至可能出现一个应用只服务几个人、被用几次就丢掉的现象，传统的App Store形态不适合承载这种散碎的软件生态。（[06:02](https://youtu.be/buYQ-_V2Wv0?t=362)）
- [[spatial-composability]] — 空间不可撤销的典型例子是：删除游戏后，当初为其安装的联机工具、MOD管理软件、甚至作弊器依然留在系统中。（[06:02](https://youtu.be/buYQ-_V2Wv0?t=362)）
- [[stock-market-plugin]] — 股票大盘插件是 DeepSeek Harness 中一个实用的副产品插件，安装后可以直接在界面里盯盘，大幅提升查看股市行情的便利性。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[temporal-composability]] — 时间不可撤销的典型例子是：删除一个游戏后，其存档配置文件以及写入注册表的各种信息依然残留在系统文件夹和注册表中。（[06:02](https://youtu.be/buYQ-_V2Wv0?t=362)）
- [[thinking-intensity-slider-plugin]] — 滑动变速器插件可以直观地调整模型思考强度的挡位，简单任务时把挡位调低，能间接达到节省 API 额度消耗的效果。（[03:01](https://youtu.be/buYQ-_V2Wv0?t=181)）
- [[traditional-software-composability-weakness]] — 传统软件体系的时间和空间可组合性普遍很差，这也是各类系统清理工具长期流行、大家早已见怪不怪的原因。（[06:02](https://youtu.be/buYQ-_V2Wv0?t=362)）
