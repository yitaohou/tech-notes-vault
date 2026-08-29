---
video_id: aR97E7aKEgg
title: 700 萬人下載的 /grill-me，Matt Pocock 到底寫了什麼？
source: '[[2026-07-22-700-萬人下載的-grill-mematt-pocock-到底寫了什麼]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: d44f17534b671375d50d27a7ebbacef49335b687e0ea12ea12dfb820fc76b681
  schema_version: 1
  model: sonnet
  generated_at: '2026-08-26T19:25:05+00:00'
---

## 一句话总结

Matt Pocock 700 万次下载的 [[grill-me-skill|grill-me]] 只有五行字，但它背后是一整套用软件工程经典理论（TDD、deep module、code smell）驯服 AI 随机性的 skill 生产线，核心思路是用精炼的专业术语当 prompt，把决策权始终留在人类手里。

## 核心内容

### 为什么要控制 AI:随机性才是难题

[[matt-pocock]] 是 TypeScript 领域最顶尖的老师，他发现写代码的速度从来不是瓶颈，真正难的是如何控制 AI 这个充满随机性的黑盒子([[ai-randomness-control-goal|00:00]])。他的 [[matt-pocock-skills-project|skills 专案]]在 GitHub 上已获得超过 16 万星、下载超过 700 万次，不只包含 [[grill-me]] 这一个 skill,还涵盖从写规格、拆任务到写测试的一整套流程(00:00)。与市面上另一套热门框架 [[superpowers-skill-framework|Superpowers]]、以及会把整个开发流程绑成一条又重又硬的固定流程的 [[spec-kit|Spec-Kit]]不同(一旦前面一步定歪,错误会顺着整条线传染,特别难中途修改),Matt 选择了完全相反的路线:[[modular-small-skill-design-philosophy|小而模组化]],每个 skill 刻意做得很小、很好改、还能自由拼装(00:00)。

### grill-me:把找漏洞的苦差事丢给 AI

[[software-development-decision-making|软件开发的本质]]是连续做出几百个微观决定,例如防呆怎么做、断线怎么办、极端资料怎么处理(03:00)。如果把模糊想法直接丢给 AI 凭感觉写代码([[vibe-coding]]),等于把这上百个决策权外包给黑盒子,AI 为了讨好用户通常会编出最难维护的架构(03:00)。[[grill-me]] 的解法是四条规则:达成共识前拚命问问题、像画心智图一样顺着用户思路挖出连锁反应、每次只问一个问题并附上建议答案、共识达成前绝不准偷跑写程式(00:00)。这套 [[ai-blind-spot-questioning|拷问式提问]]的价值在于:让人类从空白画面写出涵盖所有极端情况的完美企划书太痛苦,不如让 AI 顺着决策树无情挖出用户脑中没想清楚的盲点(03:00)。但 grill-me 的 skill 文件本身唯一目的是把决策权抢回人类手里——AI 只给选项,人类始终坐在架构师位置上拍板(03:00)。

### 从共识到代码:to-spec、to-tickets 与 TDD 生产线

对话一结束 AI 就会失忆,刚吵出来的共识直接蒸发([[ai-context-amnesia-session|03:00]]),所以生产线第二站用 [[to-spec-skill|to-spec]] 把共识写成规格书。这里有条铁律——[[to-spec-no-code-rule|绝不在规格书里写代码]],因为代码是最容易变动的部分,写进规格就会遇上 [[spec-code-staleness-problem|文件跟不上代码更新]]的老问题,下次 AI 照规格改功能时反而被过期代码搞混(03:00)。

第三站 [[to-tickets-skill|to-tickets]] 把规格拆解成待办任务,专门对付 [[ai-task-planning-weakness|AI 规划任务天生很烂]]这个弱点:AI 若自己拆分,会按 [[architecture-first-task-breakdown-flaw|技术架构分工]](先建完数据库,再写后端,最后画前端),这样最大的问题是直到最后一步前完全无法测试,一旦第一步建错,要等到最后才发现,前面心血全毁(03:00)。to-tickets 强制改用 [[feature-based-task-breakdown|按使用者功能拆分]],例如电商网站切出「会员登入」「加入购物车」,每个任务各自包含完整的资料库、后端、前端(03:00)。这样做完一个小功能就能立刻验证是否能运作([[task-decomposition-by-feature|06:00]])。to-tickets 还会自动排序,把互不干扰的任务同时[[parallel-task-dispatch-ai|平行发包给多个 AI]],开发速度直接翻倍(06:00)。

第四站 [[implement-skill]] 照任务清单写代码,过程中自动用 [[test-driven-development|TDD]] 引导:必须先写死测试跑出红灯,才允许写实现代码,直到变绿灯为止([[red-green-tdd-cycle|06:00]])。这个顺序至关重要——如果先写实现代码再补测试,AI 写错逻辑后可能为了交差生成一个必定通过的假测试,bug 就永远藏起来了([[tdd-prevents-ai-cheating|06:00]] / [[tdd-constrains-ai-cheating|15:00]])。写完测试通过后自动触发 [[code-review-skill|Code Review skill]],它会在全新 session 里审查,避免被写代码时的记忆干扰判断([[fresh-session-code-review|06:00]]),检查清单包含 [[shotgun-surgery|Shotgun Surgery]](改一个小地方却要打开十几个文件)等经典烂代码症状(06:00)。

### 用一个词代替一百句废话:pruning 与 deep module

[[writing-great-skills-skill]] 这个 skill 教 Matt 如何把提示词磨精炼,其中第三原则是 [[completion-criteria-principle|完成标准]]——给 AI 明确终点防止输出无限发散(09:00)。核心是 [[pruning-principle|pruning 原则]]:在 AI 面前多写一句废话就多一分分心可能,要修剪掉所有非必要文字(09:00)。这靠的是 [[jargon-as-compressed-instruction|指引词]]——信息被极度压缩但含金量超高的专有名词,例如说出 "Data Clumps" 就等于说了一整句检查指令(09:00)。[[code-review-skill]] 里点名的 12 种烂代码现象全部来自经典名著《[[refactoring-book|Refactoring]]》(09:00),包括 [[feature-envy|Feature Envy]](处理订单的代码却总去存货文件取数据)和 [[data-clumps|Data Clumps]](姓名、电话、地址总绑在一起就该打包成物件)(09:00)。

AI [[ai-lacks-global-view-coding|天生没有大局观]],每次只能盯着眼前几个文件,最容易写出 [[shallow-module|浅模块]]——就像分好房间却没大门的房子,进厨房要爬窗户(09:00)。浅模块对 AI 维护极不友好,因为 context window 有限,修 bug 时要在多个文件间跳转拼凑上下文,一旦逻辑超出记忆范围就会瞎猜,甚至改坏正常代码(12:00)。相对的 [[deep-module|深模块]]不是把代码硬塞进一个文件,而是建一扇极简单的大门(如 processCheckout 函数),把复杂子逻辑全部藏在门后,主程式只需敲一次门(12:00);其对 AI 友好的关键在于局部性(locality)——出问题时只需专注这一个模块即可定位修复(12:00)。判断真假深模块的方法是 [[deletion-test|删除测试]]:拔掉模块后天下大乱说明是真深模块,拔掉后代码反而更清爽则是该清理的浅模块空壳(12:00)。[[improve-codebase-architecture-skill]] 就是把这套删除测试自动化,扫描整个专案生成 HTML 诊断报告,附重构前后对比图,用户只需挑一条建议让 AI 照做(12:00)。

### 隐形炸弹与哲学落地:逻辑碎片化 vs 积木式 skill

即便整套流程把 AI 训练成顶级工程师,项目依然存在一个隐患:[[logic-fragmentation-risk|逻辑过度碎片化]](09:00)。Matt 用 [[grill-me-to-spec-skill|grill-me 搭配 to-spec]]的方式连续追问,逼出用户没说清楚的细节,防止 AI 自行猜测需求(12:00)。日常使用上,Matt 自己更常用 [[grill-with-docs]] 而非最初版的 [[grill-me]],因为 grill-me 每次开工都要重新摸索项目,前半场问题都在了解背景,真正尖锐的问题要等摸熟后才问得出来([[grill-me|15:00]]);grill-with-docs 把专有名词定义和决策原因写成文档,之后 AI 带着资料能一开场就切重点(15:00)。

[[skill-modularity-philosophy|Matt 的 skill 设计哲学]]与 Superpowers 完全相反:极简主义、模块化,一个 skill 只解决一个问题,不用固定流程绑架用户,可按当下阶段灵活选用工具(15:00)。Superpowers 用写死的九个步骤强制先想清楚目标、写好文件才准动工,这套 [[superpowers-skill-pipeline|保母级防呆流程]]在模型能力弱、容易偏题的阶段很管用(15:00),但对 GPT-5.6、Sol、Fable 5 这类理解力极强的现代模型反而是累赘(15:00)。得益于 [[skill-composability|skill 的可组合性]],[[to-tickets-skill|to-tickets]] 只要求输入是规格文件,不管来源是自己写的、主管给的还是别的 AI 产的,都能直接拆任务,无需从头走完整流程(18:01)。这体现了 [[lego-blocks-skill-design|积木式 skill 设计]]:随插即用,把工作主导权交还使用者,从哪一步开始、到哪一步结束完全自己决定(18:01)。

最终,Matt 把 [[deep-module-concept|深模块]]、[[code-smell|code smell]]等软件工程界已被验证有效的老方法融入 skill 架构,用来规范 AI 行为(18:01)。与其写一堆废话解释糟糕需求,不如直接丢一个 [[precise-terminology-as-prompt|精准专业术语]],AI 一听就懂,术语本身已精确限定执行范围,没有分心空间(18:01)。这打破了「有 AI 就不需要在专业领域精进」的迷思——[[domain-expertise-controls-ai|只有成为专业领域专家,才能真正控制好 AI]];Matt 真正开源的不是几个 skill,而是在教大家用专业领域积累的思维和语言去驾驭 AI 这个黑盒子(18:01)。

## 值得记住的细节

- [[grill-me]] 的 skill 文件实际只有五行字,四条规则:穷追不舍问到有共识、像心智图一样挖连锁反应、每次限一问且附建议答案、共识达成前绝不写代码(00:00)。
- [[matt-pocock-skills-project]] GitHub 星数超 16 万,下载超 700 万次(00:00)。
- [[code-review-skill]] 检查清单中的 12 种烂代码现象全部出自《[[refactoring-book|Refactoring]]》一书(09:00)。
- [[red-green-tdd-cycle|TDD]] 顺序不能反:先写死测试跑红灯,再写实现代码变绿灯,否则 AI 可能生成配合错误结果的假测试蒙混过关(06:00)。
- [[code-review-skill]] 会开全新 session 审查代码,避免被写代码过程的记忆干扰判断(06:00)。
- [[to-tickets-skill]] 会自动把互不干扰的任务平行发包给多个 AI 同时处理,速度可翻倍(06:00)。
- [[improve-codebase-architecture-skill]] 建议每隔几天在终端机跑一次,本机生成 HTML 诊断报告和重构前后架构对比图,不需要看代码,挑一条建议告诉 AI 照做即可(12:00)。
- [[deletion-test|删除测试]]是判断深/浅模块的具体方法:拔掉模块后代码变乱=真深模块;拔掉后代码变清爽=该清理的浅壳(12:00)。
- Matt 日常写代码更常用 [[grill-with-docs]] 而非最初版 [[grill-me]](15:00)。
- Superpowers 的九步防呆流程点名对比模型:GPT-5.6、Sol、Fable 5 这类现代模型觉得是累赘(15:00)。

## 这个视频适合谁 / 可以跳过什么

适合正在用 AI 辅助编程、苦恼于 AI 产出不受控或代码架构混乱的开发者,以及想理解「如何用专业术语和经典软件工程理论驾驭 AI」这一方法论的人。如果只想知道 grill-me 是什么、能直接看 00:00-03:00 的规则介绍和整体理念;若已熟悉 TDD、deep module、code smell 等软件工程概念,可以快进 06:00-09:00 的基础定义讲解,直接看 12:00 之后关于 deletion-test、逻辑碎片化风险和 skill 组合哲学的部分,这是本视频区别于泛泛而谈的核心洞察。
