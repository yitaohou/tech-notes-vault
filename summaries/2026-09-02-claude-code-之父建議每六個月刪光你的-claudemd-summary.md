---
video_id: Z-4AsgTYv2c
title: Claude Code 之父建議，每六個月刪光你的 CLAUDE.md？
source: '[[2026-09-02-claude-code-之父建議每六個月刪光你的-claudemd]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: 5d44f584ceda601eb7395aa05ac5d1176e42323f00ee5d4529f75a41fc0c118a
  schema_version: 1
  model: sonnet
  generated_at: '2026-09-03T14:48:42+00:00'
---

## 一句话总结

[[boris-cherny]]（Claude Code 之父）提出反直觉建议：应每六个月删光 CLAUDE.md、Skills 与 Hooks 重来，因为这些为旧模型打的补丁会随模型变强而变成拖累；作者据此用消融实验方法论，把自己三百多行的影片制作 skill 大扫除，转向"目标导向"而非"流程导向"的提示词写法。

## 核心内容

### 为什么要定期删光 Prompt

[[boris-cherny|Boris Cherny]] 在访谈中提出一个反直觉建议：应该每六个月把自己的 CLAUDE.md、Skills 与 Hooks 全部删除重来（00:00）。原因在于 [[claude-code-harness-refresh-on-model-release|Claude Code 团队并不训练模型本身，而是在模型训练完成后重新调整产品外层的 Harness 配置]]（00:00）。[[hardcoded-prompt-rules-limitation|以前 Agent 读取文件不可靠时写的绕路流程、漏格式时加的检查规则，在工具和模型都变强后依然留在提示词里，反而变成拖慢模型的阻力]]，这种提示词负债的累积过程类似公司 SOP 不断增补：员工每次出错就多加一道签核流程，几年后即使换了能力更强的新人，寄一封信仍要经过层层历史遗留的关卡（00:00）。Boris 用 [[unhobbling|Unhobbling（解开束缚）]]这个词来形容团队在新模型推出后重新调整外层 Harness 的动作，Hobble 本意是把脚绑住（00:00）。

### 三分类框架与消融实验

由于 Boris 没有给出具体分类标准，作者建议把现有 instructions 拆成三类，即 [[instruction-three-category-framework|指令三分类框架]]（03:01）：

- [[necessary-context-instruction|必要 Context]]（如品牌定位、目标受众、专案资料位置）：模型不论多强都无法通灵得知，一旦拿掉就不知道用什么资料完成任务，因此一定要留着（03:01）。
- [[safety-acceptance-boundary-instruction|安全与验收边界]]（如禁碰资料范围、需人工确认的操作、引用须附来源）：本来就不是为提升模型智力而写，不该为追求精简而删除（03:01）。
- [[workflow-control-instruction|Workflow Control]]（如强制每段列三点、工具须按固定顺序、把模型本来就会的动作写死）：最可能是为旧模型留下的补丁，是最值得优先做消融测试的一类（03:01）。即使是与品质相关的 workflow control 规则，也可能因模型能力提升而不再需要，应通过测试判断而非直接假设无用（03:01）。

具体的 [[ablation-testing-three-step-method|消融测试三步法]]（06:17）：第一步挑选最常做的任务或最常触发的 Skill，用现有设定跑几次作为对照组，记录文笔、漏填栏位、错误数量与人工调整耗时；第二步在乾净 Session 中拿掉认为可删除的 Workflow Control（保留必要 Context 与安全边界），用完全相同的任务、工具与评分方法重测；第三步观察刪减版本反复出问题的地方，先整类加回做初步筛选，若改善再拆成单条细测。因为模型输出带随机性，需要 [[multi-run-average-comparison|多次运行取平均比较]]，而不是各挑一次最好的结果来比（06:17）。若拿掉某条规则后测试结果没变差甚至更好，即可采用 [[category-then-individual-rollback-strategy|先整类、后单条的回滚策略]]，准备正式删除（06:17）。

### 实测案例：一次真实的大扫除

作者的影片制作 skill 因一年来每次模型犯错就多加几行规则，最终膨胀到三百多行，甚至包含文字九步流程图并强制规定一步都不准跳（06:17）。大扫除后，[[skill-cleanup-line-reduction-result|十五个 skill 檔案删掉两千五百多行、只加回三百多行，多数缩减到一百行以内]]（06:17）。过程中发现 Agent 有几次触碰了明确禁止的红线，因此花了约 [[cleanup-verification-workdays|两个完整工作日]]边测试边补回真正必要的规则（06:17）。这次改写的核心理念是 [[goal-over-process-instruction-philosophy|不再教 Agent 该怎么走，只告诉它要走到哪里]]，即从 [[workflow-control-to-goal-shift|流程式指令转向目标导向指令]]：不是留白，而是把"要怎么做"换成"要达成什么、不能踩哪条线、做到什么程度算完成"（06:17）。另外要注意 [[task-specific-rule-placement|任务专属规则的摆放位置]]：只在特定任务用到的规则不该放进全域 agent.md，而应归类到更精确的资料夹，比方说专属 skill（06:17）。

### 验证比 Prompt 措辞更重要

[[verification-over-prompt-tuning|Boris 认为大家花最多时间调整 prompt 措辞，但真正做错的地方是验证（verification）环节]]（09:39）。核心问题常是 [[model-needs-definition-of-good|模型给出平庸结果，往往不是模型本身的问题，而是使用者从未告诉它好的标准长什么样]]（09:39）。因此设定目标时应遵循 [[goal-with-evidence-requirement|目标+证据要求]]：不要只描述"好"是什么样子，还要指定模型必须拿出什么证据证明已达标（09:39），并满足 [[model-self-verification-requirement|模型自我验证的可行性]]——要求验证网页就要让模型真的能打开网页，要求测试通过就要让模型真的能跑测试（09:39）。对于像品牌语气、论证品质这类较主观的项目，应采用 [[subjective-criteria-fixed-rubric-or-review|固定评分标准或人工覆核]]的方式（09:39）；若标准模型无法自行验证，那它就只是空话，[[unverifiable-standard-manual-fallback|最后还是要回到使用者身上做人工检查]]（09:39）。验证标准同时也是 [[completion-criteria-principle|完成的终点标准]]：标准订在哪，模型才知道什么时候可以停，因此应明讲要求的是已测试、完整检查过、可直接上线的成品，并要求模型一直修到验证通过为止（09:39）。

### Eval 也会过期

[[benchmark-saturation|一份自建的 eval 大概只能活一到三个模型世代]]，因为模型进步太快，新 eval 出来没多久新模型就直接考满分，导致该 eval 无法再区分模型好坏，只能整份丢掉重出题（09:39）。当模型开始稳定考满分，[[eval-refresh-workflow|该做的不是庆祝，而是回头检视模型现在真正卡在哪里，把那里当作新的一组测试任务]]（09:39）。这也印证了 [[prompt-eval-not-permanent-assets|Prompt 和 Eval 都不是永久资产]]：模型更新时，指导它的 prompt 与测量它的 eval 都得跟着更新（09:39）。经过测试后真正该留下的是 [[eval-testing-final-artifacts|清楚目标、必要 context、可查证的验收方式，以及经测试确实能修复错误的少数关键规则]]，让每条控制模型行为的规则背后都有明确测试证据支持（09:39）。

### 如何判断该删还是该留

作者写了一个 [[claude-md-audit-prompt|CLAUDE.md 审查提示词]]，用来把现有设定一条一条摊开，找出模型本来就会、根本不用写的规则（12:47）。判断的两个自检问题体现 [[pruning-principle|删减原则]]与 [[self-discoverable-info-pruning|可自行发现信息的删减原则]]：这句话有没有真的改变模型行为（没改变就是在吃 context，可删）；这件事 AI 自己查不查得到（如专案结构、可用指令，AI 读一下就知道，不需抄进提示词）（12:47）。真正值得保留的是 [[prompt-retain-tacit-conventions|模型查不到的不成文惯例，以及某个决定背后的原因]]（12:47）。要认识到 [[prompt-depreciation-over-model-versions|一条 Prompt 曾经有效只能证明它当时解决过问题，不代表永久有效]]，因为模型会不断更新变强（12:47）。多数人建立 AI workflow 时容易陷入 [[prompt-additive-accumulation-antipattern|只增不减的堆积反模式]]，犯一个错误就写进 prompt，例外处理和错误范例久而久之堆积如山（12:47）。Boris 建议采用 [[empirical-failure-driven-prompt-diagnosis|以实证失败驱动的诊断方式]]：与其把网络技巧全塞进设定，不如先让模型执行真实且够难的任务，观察它反复失败之处，再决定补 Prompt、加 Skill 还是接 MCP（12:47）。最终指向 [[mature-workflow-minimal-rules-principle|成熟工作流的极简规则原则]]：不是靠规则数量取胜，而是让每条规则简单扼要地定义目标，留给模型足够发挥空间（12:47）。

## 值得记住的细节

- Boris Cherny 建议每六个月重做一次 CLAUDE.md、Skills、Hooks（00:00）
- 三分类框架：必要 Context / Workflow Control / 安全与验收边界，优先对 Workflow Control 做消融测试（03:01）
- 消融测试三步：对照组测试 → 拿掉规则重测（乾净 Session，保留 Context 与安全边界）→ 整类加回筛选再拆单条（06:17）
- 因输出随机性，须多次运行取平均值比较，不能各挑一次最好结果（06:17）
- 实测结果：15 个 skill 档案删掉 2500+ 行，仅加回 300+ 行，多数缩到 100 行以内（06:17）
- 清理后花了约 2 个完整工作日核实并补回真正必要的规则（06:17）
- 一份自建 eval 大约只能撑 1-3 个模型世代就会饱和（09:39）
- 设定验证标准时要确保模型真的有能力自行核实（如真的能打开网页、真的能跑测试）（09:39）
- 主观项目（品牌语气、论证品质）用固定评分标准或人工覆核，而非要求模型自证（09:39）
- 陷阱：任务专属规则若放进全域 agent.md/claude.md，会污染其他任务的 context，应放到专属 skill 资料夹（06:17）
- 自检两问：这句话是否真的改变模型行为？这件事 AI 自己查不查得到？两者皆否则可删（12:47）

## 这个视频适合谁 / 可以跳过什么

适合已经用 Claude Code / CLAUDE.md 一段时间、感觉提示词越写越臃肿、workflow 变慢的人，尤其是想学习系统化消融测试方法而非凭感觉删减的开发者。如果你还没建立起自己的 CLAUDE.md 或 Skills 体系，或者不使用 Agent 编码工具，可以跳过；此外如果只想要"结论"，可以直接看 06:17 之后的实测案例与 12:47 的审查提示词方法，跳过前段关于 Unhobbling 概念的铺垫（00:00-03:01）。
