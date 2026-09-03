---
video_id: Z-4AsgTYv2c
url: https://www.youtube.com/watch?v=Z-4AsgTYv2c
title: Claude Code 之父建議，每六個月刪光你的 CLAUDE.md？
channel: Gary Chen
published: '2026-09-02'
duration: '15:04'
transcript_origin: subs
tags:
- video
---

# Claude Code 之父建議，每六個月刪光你的 CLAUDE.md？

摘要: [[2026-09-02-claude-code-之父建議每六個月刪光你的-claudemd-summary|完整摘要]]

## 知识点

- [[ablation-study-prompt-testing]] — Boris 提到 Claude Code 团队用消融实验（ablation study）来判断某条 Prompt 规则是否还有必要：拿掉一个变因、保持其他条件不变，再比较结果是变好、变差还是没有影响。（[03:01](https://youtu.be/Z-4AsgTYv2c?t=181)）
- [[ablation-testing-three-step-method]] — Ablation 测试第一步是挑选最常做的任务或最常触发的 Skill，用现有设定跑几次作为对照组，记录文笔、漏填栏位、错误数量与人工调整所花的总时间。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
- [[benchmark-saturation]] — Boris Cherny 提到，一份自建的 eval 大概只能活一到三个模型世代，因为模型进步太快，往往新 eval 出来没多久新模型就直接考满分，导致这份 eval 再也无法区分模型好坏，只能整份丢掉重新出题。（[09:39](https://youtu.be/Z-4AsgTYv2c?t=579)）
- [[boris-cherny]] — Boris Cherny 在一场访谈中提出反直觉建议：应该每六个月把自己的 CLAUDE.md、Skills 与 Hooks 全部删除重来。（[00:00](https://youtu.be/Z-4AsgTYv2c?t=0)）
- [[category-then-individual-rollback-strategy]] — 如果拿掉某条规则后测试结果不但没有变差、甚至还变得更好，那这条规则就可以准备正式删除。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
- [[claude-code-harness-refresh-on-model-release]] — Claude Code 团队不是训练模型本身，而是在模型训练完成、推出之后重新调整产品外层的 Harness 配置。（[00:00](https://youtu.be/Z-4AsgTYv2c?t=0)）
- [[claude-md-audit-prompt]] — 作者在清理过程中顺手写了一个提示词，用来把现有的 CLAUDE.md 和 Skills 一条一条摊开，找出那些模型本来就会、根本不用写的规则。（[12:47](https://youtu.be/Z-4AsgTYv2c?t=767)）
- [[cleanup-verification-workdays]] — 大扫除过程中作者发现 Agent 有几次触碰了明确禁止的红线，因此花了约两个完整工作日边测试边把真正必要的规则补回来。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
- [[completion-criteria-principle]] — 验证标准同时也是完成终点：标准订在哪，模型才知道什么时候可以停，因此应明讲要求的不是原型或概念验证，而是已测试、反复修改过、完整检查过、可直接上线的成品，并要求模型一直修到验证通过为止。（[09:39](https://youtu.be/Z-4AsgTYv2c?t=579)）
- [[empirical-failure-driven-prompt-diagnosis]] — Boris 认为与其把网络上看到的各种技巧全部塞进设定，不如先让模型执行一个真实且够难的任务，观察它反复失败的地方，再据此决定要补充 Prompt、加 Skill，还是接上 MCP。（[12:47](https://youtu.be/Z-4AsgTYv2c?t=767)）
- [[eval-refresh-workflow]] — 当模型开始在 eval 上稳定考满分，该做的不是庆祝，而是回头检视模型现在真正卡在哪里，把那个地方当作新的一组测试任务。（[09:39](https://youtu.be/Z-4AsgTYv2c?t=579)）
- [[eval-testing-final-artifacts]] — 经过 eval 测试后真正该留下来的是：清楚的目标、必要的 context、能查证结果的验收方式，以及经过反复测试确实能修复错误的少数关键规则，让每条控制模型行为的规则背后都有明确的测试证据支持，才能用最精简的 prompt 发挥模型最大潜力。（[09:39](https://youtu.be/Z-4AsgTYv2c?t=579)）
- [[goal-over-process-instruction-philosophy]] — 这次改写的核心理念是不再教 Agent 该怎么走，只告诉它要走到哪里，即从流程式指令转向目标导向指令。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
- [[goal-with-evidence-requirement]] — 在设定目标时不要只描述『好』是什么样子，还要指定模型必须拿出什么证据来证明它已经达标。（[09:39](https://youtu.be/Z-4AsgTYv2c?t=579)）
- [[hardcoded-prompt-rules-limitation]] — 以前 Agent 读取文件不可靠时写的绕路流程、漏格式时加的检查规则，在工具和模型都变强后依然留在提示词里，反而变成拖慢模型的阻力。（[00:00](https://youtu.be/Z-4AsgTYv2c?t=0)）
- [[instruction-three-category-framework]] — 由于 Boris 没有给出具体分类标准，建议把现有 instructions 拆分成必要 Context、Workflow Control、安全与验收边界三类，再分别判断是否值得做消融测试。（[03:01](https://youtu.be/Z-4AsgTYv2c?t=181)）
- [[mature-workflow-minimal-rules-principle]] — 一套真正成熟的 workflow 不是靠规则数量取胜，而是要让每条规则都简单扼要地定义目标，并留给模型足够的发挥空间。（[12:47](https://youtu.be/Z-4AsgTYv2c?t=767)）
- [[model-needs-definition-of-good]] — 模型给出平庸结果时，问题往往不在模型本身，而是使用者从未告诉过它好的标准长什么样，模型自然做不出好东西。（[09:39](https://youtu.be/Z-4AsgTYv2c?t=579)）
- [[model-self-verification-requirement]] — 设定验证标准时必须让模型有能力自行核实：要求验证网页就要让模型真的能打开网页，要求测试通过就要让模型真的能跑测试，要求引用来源就要让模型真的能点开原始连结。（[09:39](https://youtu.be/Z-4AsgTYv2c?t=579)）
- [[multi-run-average-comparison]] — 因为模型输出带有随机性，同一组任务在新旧设定下都必须各跑几次，比较的是这两个版本在多次测试中的平均表现、失败率与稳定度，而不是各挑一次最好的结果来比。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
- [[necessary-context-instruction]] — 必要 Context 类的 instructions（如品牌定位、目标受众、专案资料位置）不论模型多强都无法通灵得知，一旦拿掉模型就不知道该用什么资料完成任务，因此这类设定一定要留着。（[03:01](https://youtu.be/Z-4AsgTYv2c?t=181)）
- [[prompt-additive-accumulation-antipattern]] — 多数人建立 AI workflow 时往往只增不减，犯一个错误就写进 prompt 里，久而久之这些例外处理和错误范例就堆积如山。（[12:47](https://youtu.be/Z-4AsgTYv2c?t=767)）
- [[prompt-depreciation-over-model-versions]] — 一条 Prompt 曾经有效只能证明它在当时解决过问题，并不代表它永久有效，因为模型会不断更新、变得越来越强大。（[12:47](https://youtu.be/Z-4AsgTYv2c?t=767)）
- [[prompt-eval-not-permanent-assets]] — Prompt 和 Eval 都不是永久资产，模型更新的时候，用来指导它的 prompt 与用来测量它的 eval 都得跟着一起更新。（[09:39](https://youtu.be/Z-4AsgTYv2c?t=579)）
- [[prompt-retain-tacit-conventions]] — 真正值得写进提示词的内容，是模型查不到的那些不成文的惯例，以及某个决定背后的原因。（[12:47](https://youtu.be/Z-4AsgTYv2c?t=767)）
- [[pruning-principle]] — 判断提示词中某条规则是否该保留的自检问题之一：这句话有没有真的改变模型的行为，如果模型本来就会这样做，这句话就只是在吃掉 context，可以直接删掉。（[12:47](https://youtu.be/Z-4AsgTYv2c?t=767)）
- [[safety-acceptance-boundary-instruction]] — 安全与验收边界类的 instructions（如禁碰资料范围、需人工确认的操作、引用须附来源、发布条件）本来就不是为了提升模型智力而写，因此不该为了追求 Prompt 精简而在真实工作环境中直接删除。（[03:01](https://youtu.be/Z-4AsgTYv2c?t=181)）
- [[self-discoverable-info-pruning]] — 第二个自检问题是这件事 AI 自己查得到吗，例如专案结构、有哪些指令可以用，AI 读一下就知道，不需要额外抄一份写进提示词。（[12:47](https://youtu.be/Z-4AsgTYv2c?t=767)）
- [[skill-cleanup-line-reduction-result]] — 作者把影片制作 pipeline 的十五个 skill 檔案大扫除后，删掉两千五百多行、只加回三百多行，多数 skill 缩减到一百行以内。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
- [[subjective-criteria-fixed-rubric-or-review]] — 像品牌语气、论证品质这类较主观的项目，模型难以自行验证，应固定一套评分标准，或者直接交给人工覆核。（[09:39](https://youtu.be/Z-4AsgTYv2c?t=579)）
- [[task-specific-rule-placement]] — 如果某条规则只有在特定任务才会用到，就不该把它放在全域的 agent.md 或 claude.md 里，而应该归类到更精确的资料夹底下，比方说专属的 skill。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
- [[unhobbling]] — Boris Cherny 用 Unhobbling（解开束缚）这个词来形容 Claude Code 团队在新模型推出后重新调整外层 Harness 的动作，Hobble 本意是把脚绑住。（[00:00](https://youtu.be/Z-4AsgTYv2c?t=0)）
- [[unverifiable-standard-manual-fallback]] — 如果一个标准是模型无法自行验证的，那它就只是一句空话，最后还是要回到使用者身上做人工检查。（[09:39](https://youtu.be/Z-4AsgTYv2c?t=579)）
- [[verification-over-prompt-tuning]] — Boris Cherny 认为，大家花最多时间调整 prompt 措辞，但真正做错的地方是验证（verification）环节，而非 prompt 写得漂不漂亮。（[09:39](https://youtu.be/Z-4AsgTYv2c?t=579)）
- [[workflow-control-instruction]] — Workflow Control 类规则（如强制每段列三点、工具必须按固定顺序使用、把模型本来就会的动作写死）最可能是为旧模型留下的补丁，因此是最值得优先做消融测试的一类。（[03:01](https://youtu.be/Z-4AsgTYv2c?t=181)）
- [[workflow-control-to-goal-shift]] — 删除 Workflow Control 并不是留白，而是把「要怎么做」换成「要达成什么、不能踩哪条线、做到什么程度算完成」。（[06:17](https://youtu.be/Z-4AsgTYv2c?t=377)）
