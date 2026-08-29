---
video_id: aR97E7aKEgg
url: https://www.youtube.com/watch?v=aR97E7aKEgg
title: 700 萬人下載的 /grill-me，Matt Pocock 到底寫了什麼？
channel: Gary Chen
published: '2026-07-22'
duration: '20:01'
transcript_origin: subs
tags:
- video
---

# 700 萬人下載的 /grill-me，Matt Pocock 到底寫了什麼？

摘要: [[2026-07-22-700-萬人下載的-grill-mematt-pocock-到底寫了什麼-summary|完整摘要]]

## 知识点

- [[ai-blind-spot-questioning]] — 让人类从空白画面写出涵盖所有极端状况的完美企划书太痛苦，所以 grill-me 把找漏洞的苦差事丢给 AI，由 AI 顺着决策树无情挖出用户脑中没想清楚的盲点。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
- [[ai-context-amnesia-session]] — 用户被 grill-me 拷问完达成共识后，只要一关掉对话，AI 就会立刻失忆，刚才吵出来的共识直接蒸发，因此需要额外一步把共识写下来保存。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
- [[ai-lacks-global-view-coding]] — AI 写程式的速度实在太快，但它天生没有大局观，每次只能盯着眼前的那几个文件，为了方便交差最容易写出所谓的浅模块。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
- [[ai-limited-memory-concise-prompts]] — AI 的记忆有限，因此需要用精炼的引导词或专业名词与之沟通，而非冗长的自然语言描述。（[15:00](https://youtu.be/aR97E7aKEgg?t=900)）
- [[ai-randomness-control-goal]] — Matt Pocock 发现，比起写 code 的速度，更难的是怎么控制 AI，因为 AI 本质上是一个充满随机性的黑盒子。（[00:00](https://youtu.be/aR97E7aKEgg?t=0)）
- [[ai-task-planning-weakness]] — to-tickets 这个 skill 蕴含的开发方法论专门用来对付 AI 规划任务总是很烂这个致命缺点：如果让 AI 自己决定待办清单，它天生有按照技术架构来分工的坏习惯。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
- [[architecture-first-task-breakdown-flaw]] — 举例来说，如果让 AI 自己规划一个电商网站的任务，它会先把全部资料库建好，再把处理资料的后端逻辑写完，最后才画出前端画面；这样拆分最可怕的盲点是，在最后一步画面出来之前完全没办法测试任何东西，如果第一步资料库建错了，要等到做前端画面时才会发现，前面的心血就全毁了。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
- [[code-review-skill]] — implement skill 写完代码、测试通过后会自动触发 Code Review skill，它不是只写一句空泛的『请检查有没有 Bug』，而是把软件工程界公认的烂 code 症状全部写成具体检查清单。（[06:00](https://youtu.be/aR97E7aKEgg?t=360)）
- [[code-smell]] — Matt 也把烂 code 的徵兆（code smell）这类软件工程经验方法融入 skill 架构中，作为规范 AI 行为的依据之一。（[18:01](https://youtu.be/aR97E7aKEgg?t=1081)）
- [[completion-criteria-principle]] — writing-great-skills 的第三个原则叫完成标准，即给 AI 一个明确的终点，防止它的输出无限发散。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
- [[data-clumps]] — 如果买家姓名、电话、地址这几个变量总是绑在一起出现，就应该把它们打包成一个如「联络人」的物件，而不是每次都在代码里散着传来传去，这种现象叫做 Data Clumps。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
- [[deep-module]] — 深模組不是要求把大量代码硬塞进同一个文件不准拆分，而是要蓋一扇极简单的大门（如 processCheckout 函数），把折扣计算、信用卡验证等复杂子逻辑全部藏在门后，主程式只需敲一次门即可完成整个结帐流程。（[12:00](https://youtu.be/aR97E7aKEgg?t=720)）
- [[deep-module-concept]] — Matt 把软件工程界已被证明有效的老方法，例如深模块（deep module），融入到 skill 的架构设计中，用来规范 AI 的行为。（[18:01](https://youtu.be/aR97E7aKEgg?t=1081)）
- [[deep-module-design]] — 用架构大扫除类工具审查代码，可以引导 AI 设计出接口简单、易维护的深模块。（[15:00](https://youtu.be/aR97E7aKEgg?t=900)）
- [[deletion-test]] — 如果拔掉某模块后天下大乱、原本隐藏的复杂逻辑全部炸回主程式，说明这是真正有在做事的深模組；如果拔掉后代码反而变清爽、原本要跳着看的两个文件合并到一处，说明这个模块只是没有隐藏任何细节的淺模組空壳，应该清理掉。（[12:00](https://youtu.be/aR97E7aKEgg?t=720)）
- [[domain-expertise-controls-ai]] — Matt Pocock 的案例打破了「有 AI 就不需要在专业领域精进」的迷思：只有成为专业领域的专家，才能真正控制好 AI。（[18:01](https://youtu.be/aR97E7aKEgg?t=1081)）
- [[feature-based-task-breakdown]] — 为解决按技术架构拆分任务的问题，to-tickets 强制 AI 改用使用者功能来拆任务：例如电商网站会切出「会员登入」和「加入购物车」两个任务，每个任务都各自包含专属的完整资料库、后端逻辑与前端画面。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
- [[feature-envy]] — 如果处理订单的代码总是跑去存货相关文件里取数据来算，就说明这段逻辑放错了位置，应该搬去订单自己的文件里，这种代码异味叫做 Feature Envy。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
- [[fresh-session-code-review]] — Code Review skill 会开一个全新的 session 来审查代码，这样做是为了让 AI 保持最干净、最聪明的状态，避免被写代码时留下的记忆干扰判断。（[06:00](https://youtu.be/aR97E7aKEgg?t=360)）
- [[grill-me]] — grill-me 这个被数百万人下载的 skill，实际文件内容只有短短五行字。（[00:00](https://youtu.be/aR97E7aKEgg?t=0)）
- [[grill-me-skill]] — grill-me 这个 skill 里的五行字唯一目的是把决策权抢回人类手里：AI 负责顺着决策树挖出用户脑中没想清楚的盲点、只给选项，人类始终坐在架构师的位置上拍板定案。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
- [[grill-me-to-spec-skill]] — AI 很容易自行猜测需求，做出与使用者想象不同的结果，Matt 因此用 grill-me 搭配 to-spec 的方式，透过连续追问逼出使用者原本没说清楚的细节。（[12:00](https://youtu.be/aR97E7aKEgg?t=720)）
- [[grill-with-docs]] — grill-with-docs 解决了 grill-me 每次都要重新摸索项目的痛点：程序码翻不到的专有名词定义和决策原因会被写成文档，之后 AI 带着这些资料拷问能一开场就切入重点。（[15:00](https://youtu.be/aR97E7aKEgg?t=900)）
- [[implement-skill]] — implement skill 接到实作指令后会照着任务清单开始写代码，过程中自动用 TDD 方式引导开发，写完还会自动呼叫 Code Review skill 做审查。（[06:00](https://youtu.be/aR97E7aKEgg?t=360)）
- [[improve-codebase-architecture-skill]] — improve-codebase-architecture 这个 skill 不是单纯检查语法，而是对代码库中每一个模块执行「刪除测试」，以此判断该模块究竟是深模組还是多余的淺模組空壳。（[12:00](https://youtu.be/aR97E7aKEgg?t=720)）
- [[jargon-as-compressed-instruction]] — 指引词是信息被极度压缩但含金量超高的专有名词，例如对 AI 说出 Data Clumps 这个词，就等于说了一整句「请检查代码里有没有总绑在一起出现的变量，有的话打包成独立物件」，用一个字取代一百字的废话解释。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
- [[lego-blocks-skill-design]] — 在模型越来越聪明的现在，Matt 给出的是随插即用的积木式 skill，把工作的主导权交还给使用者，从哪一步开始写程序、到哪一步结束完全自己决定。（[18:01](https://youtu.be/aR97E7aKEgg?t=1081)）
- [[logic-fragmentation-risk]] — 即使 Matt Pocock 用整套流程把 AI 训练成了顶级工程师，项目依然存在一个致命的隐形炸弹，叫做逻辑过度的碎片化。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
- [[matt-pocock]] — Matt Pocock 是 TypeScript 领域最顶尖的专家和老师，非常多开发者都是靠他的教材把技术练起来的。（[00:00](https://youtu.be/aR97E7aKEgg?t=0)）
- [[matt-pocock-skills-project]] — 该专案在 GitHub 上已获得超过 16 万颗星，被下载超过 700 万次。（[00:00](https://youtu.be/aR97E7aKEgg?t=0)）
- [[matt-pocock-writing-skills]] — 常见的 AI 写作方式是直接让 GPT 之类模型一次性生成一篇 blog 或影片脚本，而 Matt Pocock 的写作 skill 完全走另一条不同的工作流路线。（[15:00](https://youtu.be/aR97E7aKEgg?t=900)）
- [[modular-small-skill-design-philosophy]] — 与 Spec-Kit 相反，Matt Pocock 让每个 skill 刻意做得很小、很好改、还能自由拼装，这个「小而模组化」的理念是他整套专案背后的底层逻辑。（[00:00](https://youtu.be/aR97E7aKEgg?t=0)）
- [[parallel-task-dispatch-ai]] — to-tickets 会自动排好任务顺序，把互不干扰的任务同时发包给好几个 AI 平行处理，开发速度可以直接翻倍。（[06:00](https://youtu.be/aR97E7aKEgg?t=360)）
- [[precise-terminology-as-prompt]] — 与其写一大堆废话向 AI 解释糟糕的需求，不如直接丢一个精准的专业术语，AI 一听就懂，就像资深教练给球员的一句话，简单却蕴含数十年经验。（[18:01](https://youtu.be/aR97E7aKEgg?t=1081)）
- [[pruning-principle]] — Pruning 原则的核心理念是，在 AI 面前多写一句废话，AI 就多一分分心的可能，因此要修剪掉所有非必要文字，哪怕是模型自己也知道该怎么做的指令。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
- [[red-green-tdd-cycle]] — TDD 要求先把测试写死并跑出失败的红灯，才允许开始写真正的实现代码，直到测试通过变成绿灯为止，用这种顺序彻底锁死 AI 亂写交差的空间。（[06:00](https://youtu.be/aR97E7aKEgg?t=360)）
- [[refactoring-book]] — Matt Pocock 的 code review skill 中点名的 12 种烂 code 现象，全部来自经典名著《Refactoring》。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
- [[shallow-module]] — 结帐系统被拆成计算折扣、验证信用卡、建立订单、扣除库存、寄信五个小模块，却没有为这五个模块建立统一的大门来隐藏细节，导致主程式必须亲自处理五个模块间的资料传递，这是典型的淺模組设计。（[12:00](https://youtu.be/aR97E7aKEgg?t=720)）
- [[shotgun-surgery]] — Shotgun Surgery 是指明明只想改一个按钮颜色这样的小改动，结果却要打开十几个不同文件去修改，Code Review skill 会要求把这些散落的改动重新集中起来。（[06:00](https://youtu.be/aR97E7aKEgg?t=360)）
- [[skill-composability]] — to-tickets 这类 skill 只要求输入是一份规格文件，不管这份规格是自己写的、主管给的还是别的 AI 产的，都能直接丢给它拆任务，无需从头走完整流程。（[18:01](https://youtu.be/aR97E7aKEgg?t=1081)）
- [[skill-modularity-philosophy]] — Matt Pocock 的 skill 设计哲学与 Superpowers 完全相反，走极简主义与模块化路线，坚持一个 skill 只解决一个问题。（[15:00](https://youtu.be/aR97E7aKEgg?t=900)）
- [[software-development-decision-making]] — 软件开发的本质是连续做出几百个微观决定，例如防呆怎么做、断线怎么办、极端资料怎么处理。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
- [[spec-code-staleness-problem]] — 软件工程界最大的痛之一是文件永远跟不上程式码更新的速度，比起整体业务逻辑，具体的程式码是最容易变动的部分。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
- [[spec-kit]] — Spec-Kit 的问题在于把整个开发流程接管、绑成一条又重又硬的固定流程，只要前面一步定歪，错误就会顺着整条线传染到后面，特别难中途修改。（[00:00](https://youtu.be/aR97E7aKEgg?t=0)）
- [[superpowers-skill-framework]] — Superpowers 是市面上另一套试图控制 AI 开发随机性的热门框架，与 Get Shit Done、Spec-Kit 并列。（[00:00](https://youtu.be/aR97E7aKEgg?t=0)）
- [[superpowers-skill-pipeline]] — 在模型还很笨的时候，Superpowers 给出的是已经组好的自动化生产线，能确保不漏步骤、品质稳定，但产出文件是为自己下一步量身打造的，别人很难中途接手。（[18:01](https://youtu.be/aR97E7aKEgg?t=1081)）
- [[task-decomposition-by-feature]] — 按功能拆分任务的好处是每做完一个小功能就能立刻确认它能否运作，不用等几千行代码全部写完才开始审核 AI 的产出。（[06:00](https://youtu.be/aR97E7aKEgg?t=360)）
- [[tdd-constrains-ai-cheating]] — AI 容易在实现代码时作弊，用 TDD 的方式先定义好测试，能有效约束 AI 的行为边界。（[15:00](https://youtu.be/aR97E7aKEgg?t=900)）
- [[tdd-prevents-ai-cheating]] — 如果先让 AI 写实现代码再补测试，AI 写错逻辑后可能会为了交差直接生成一个配合错误结果、必定通过的假测试，导致 bug 无法被发现。（[06:00](https://youtu.be/aR97E7aKEgg?t=360)）
- [[test-driven-development]] — 测试是一段用来检查程序对错的程序，例如提前定下『购物车满 1000 元结帐必须扣 100』这条规则，之后谁改坏了逻辑测试就会立刻报错拦截。（[06:00](https://youtu.be/aR97E7aKEgg?t=360)）
- [[to-spec-no-code-rule]] — Matt 在 to-spec 这个 skill 里完全禁止 AI 在写规格书时引用或写任何程式码，因为一旦程式码写进规格、日后代码变动就会跟规格对不上，下次 AI 照规格修改功能时会被过期错误的旧代码搞混、越改越乱。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
- [[to-spec-skill]] — 为了应对 AI 对话结束后共识消失的问题，生产线第二站使用 to-spec 这个 skill，把刚才吵出来的共识写下来变成一份规格书存起来。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
- [[to-tickets-skill]] — 规格书写好之后，第三个 skill to-tickets 的作用是把上一步写出的规格书拆解成具体的待办任务。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
- [[vibe-coding]] — 把模糊想法直接丢给 AI 凭感觉写代码（vibe coding）等于把上百个微观决策权外包给 AI 这个黑盒子，而 AI 为了讨好用户通常会编出一套最难维护的架构，这是生产级软件的噩梦。（[03:00](https://youtu.be/aR97E7aKEgg?t=180)）
- [[writing-great-skills-skill]] — Matt Pocock 项目里藏着一个叫 writing-great-skills 的 skill，专门用来指导如何把提示词磨得精炼。（[09:00](https://youtu.be/aR97E7aKEgg?t=540)）
