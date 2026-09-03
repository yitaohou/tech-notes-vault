---
video_id: WrwA7FYGPdQ
title: DeepSeek Harness 开源 11 天爆 5 个漏洞：AI 读网页电脑被控，有人 API 额度已被盗刷 | QVD-2026-57410 CVSS9.
source: '[[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度]]'
tags:
- summary
_gen:
  prompt_hash: 209b52739480c30c61b7dcc0392dfa4aa0deb99654ee921af5e045409c961f85
  task_hash: d0a7ff22611a0f2e5507618f2fccac3cda56239ba8fa2733bf8c05b281e77244
  schema_version: 1
  model: sonnet
  generated_at: '2026-09-03T14:23:30+00:00'
---

## 一句话总结

DeepSeek Harness 开源仅一天就爆出4个漏洞（2个严重级别），11天内累计曝出5个漏洞，其中最严重的[[deepseek-harness-cve-2026-57410|CVSS 9.8分漏洞]]让攻击者无需窃取密钥、无需接触对话，仅凭一段公开脚本就能远程在受害者电脑上执行任意命令——这暴露出 agent 框架"快速迭代期"下安全边界的极度不稳定。

## 核心内容

### Agent 与 Harness 是什么

DeepSeek 官方给出的公式是 [[agent-model-harness-formula|agent = model + harness]]：model 负责语言理解和决策，harness 负责把决策转化为实际操作（00:00）。只能对话回复的 AI 叫 chatbot，套上 [[deepseek-harness]] 后能读写文件、执行命令、调用外部工具的才叫 [[agent-definition|agent]]（00:00）。[[deepseek-harness]] 秉持"[[deepseek-harness-everything-is-plugin|一切皆插件]]"理念，模型、工具、[[deepseek-harness-three-tier-sandbox|沙箱]]、界面甚至主循环逻辑都是可插拔组件（00:00）。安装很简单：装好 Node.js、执行一条命令即打开本机3080端口的网页界面，配置好 API 密钥和[[deepseek-harness-workspace-scope|工作区]]后即可使用（00:00）。框架提供[[deepseek-harness-modes|四种运行模式]]：标准模式、PTC模式、[[deepseek-harness-batch-script-mode|批量脚本模式]]（减少多轮交互 token 消耗）、[[deepseek-harness-mechanical-mode|机械模式]]（限定命令行和文件编辑，用于跑分）、[[deepseek-harness-creative-mode|创造模式]]（允许动态生成新工具）（03:00）。框架自带的[[deepseek-harness-trajectory-log|轨迹日志]]是一大亮点：[[trajectory-log-append-only|只能追加不能篡改]]，支持[[deepseek-harness-replay-branch-debugging|完整回放和分支重跑]]，这种[[replayable-audit-log-rare-capability|可回放审计能力]]在同类产品中很少见（03:00, 33:14）。

### 四个基础漏洞：从配置执行到沙箱逃逸

开源当天，一位独立研究员一次性披露4个漏洞并附带[[poc-exploit-code-disclosure|PoC 验证代码]]，官方安全库当天全部收录验证（06:02）。第一个是[[yaml-config-arbitrary-code-execution-vuln|配置加载任意代码执行]]：YAML 支持特殊标签语法 [[yaml-js-tag-syntax|!!js]]，[[deepseek-harness-config-code-execution|Harness 解析配置时会把值当 JS 代码在加载瞬间直接执行]]，且触发时机早于沙箱和审批机制初始化，任何防护都不起作用（06:02, 09:04）。第二个是[[docker-sandbox-info-leak-vuln|Docker 沙箱信息泄露]]。第三个是[[vm-sandbox-escape-vuln|VM 沙箱逃逸]]：[[deepseek-harness-vm-sandbox|VM 沙箱]]本应让插件代码只能通过接口调用宿主服务，但[[execute-agent-context-leak|动态加载的插件被直接传入包含宿主服务引用的 Execute Agent Context 对象]]，且未经隔离检查，验证中恶意插件借此直接读出了预设的机密字符串（09:04）。根因在于[[context-object-security-bypass|权限检查被安放在服务调用路径半路而非入口处]]：插件正常走接口会被拦截，直接窃取整个上下文对象就能绕过（12:04）。第四个漏洞是[[chained-sandbox-escape-rce-vuln|链式沙箱逃逸]]，把前三个串联，使 [[subprocess-service-host-privilege-escalation|VM 沙箱内插件调用 subprocess.spawn 在主机上直接执行命令]]，达成 [[remote-code-execution-definition|RCE]]（06:02, 09:04, 12:04）。攻击的入口可以是 [[prompt-injection-attack|prompt injection]]：借助 [[hidden-text-prompt-injection-technique|隐藏在网页源码/元数据中、对人不可见对 AI 可见的指令]]，[[prompt-injection-to-plugin-execution-chain|无需任何权限或凭据，只要让 AI 读取一段恶意内容即可触发]] cordis define/run 插件执行链（12:04, 15:05）。攻击者拿到执行权限后还能 [[config-file-backdoor-persistence|改写配置文件植入后门]]，重启电脑也无法清除（15:05）。

### 无认证管理接口：CVSS 9.8 的第五个漏洞

第五个漏洞影响最新 0.11 rc2 版本，[[cvss-severity-score|CVSS 高达 9.8 分]]（15:05）。根因是 [[deepseek-harness-unauthenticated-management-api|管理接口完全没有认证机制]]，官方文档也承认加密认证不在第一版范围内（18:07）；[[deepseek-harness-management-api-exposure|60多个高权限管理功能对外暴露]]，[[todo-placeholder-security-gap|工具执行模块代码里还留着"权限功能待实现"的 TODO]]，[[unwired-approval-service-vulnerability|审批服务功能存在但未接入默认调用链路]]（15:05）。判断请求是否来自本机的方式是检查 [[host-header-localhost-check-bypass|HTTP Host 字段是否等于 localhost]]，而这个字段完全可由客户端伪造，[[host-header-spoofing-localhost-bypass|攻击者从外网把 Host 改成 localhost 即可让服务端误判为本机请求]]（15:05, 18:07）。完整[[deepseek-harness-exploit-chain|利用链]]：第一步注册假模型提供者指向攻击者服务器；第二步触发新对话让 Harness 连接假模型；第三步假模型以工具调用指令下发命令，Harness 按指令在受害者机器上以受害者权限执行（18:07）。全程 [[attack-bypasses-api-key|完全不使用受害者的 API 密钥]]（18:07）。默认情况下 [[deepseek-harness-loopback-binding-limitation|只监听 127.0.0.1，挡住远程但挡不住同机其他恶意程序]]（18:07, 24:08）；[[deepseek-harness-exposure-methods|云服务器端口映射或反向代理绑域名]]会把管理接口暴露到公网（18:07, 24:08）。该漏洞早在8月14日就有人在 GitHub 公开审计并给出修复建议，但[[deepseek-harness-vulnerability-disclosure-gap|因缺少私密上报通道只能公开发布，此后一直无人修复]]（18:07, 21:08）。[[dsh2-shell-exploit-tool|dsh2 shell 利用脚本]]于8月20日上线，[[dsh2-shell-vulnerability-weaponization|使漏洞被工具化]]，还带批量扫描全网暴露服务的能力（18:07, 21:08）。从公开到 [[qi-anxin-cvss-rating-delay|奇安信正式定级 9.8 分中间隔了10天]]，这10天漏洞持续被大规模利用（21:08）。[[harness-rapid-iteration-security-instability|整个处置过程反映出该类框架仍处于快速施工期，安全边界一天一个样]]（21:08）。

### 腾讯朱雀实验室的14560次真实测评

[[tencent-zhuque-lab-security-assessment|腾讯朱雀实验室]]跑了14,560次测试。结果显示 [[injection-attack-say-vs-do-asymmetry|"说出秘密"比"真正动手执行"容易得多]]：诱导说出预置假机密的 [[information-extraction-attack|信息泄露测试成功率35.7%]]，而诱导真正调用敏感工具的 [[agentic-write-actions|写操作测试成功率仅2.5%]]（21:08）。但作者提醒，2.5%在大规模调用场景下仍会产生相当数量的成功攻击，不能视为绝对安全（21:08）。更关键的发现是 [[plaintext-injection-testing-blindspot|"只测纯文本会漏掉真实攻击行为"]]：指令直接写在正文中，455次测试成功率为0%全部被防住；但 [[hidden-injection-payload-location|藏进 PDF 元数据、表格单元格或 Unicode 零宽字符后，成功率从0%跳到25.5%]]（21:08）。综合全部约14000多处组合测试，[[deepseek-harness-injection-success-rate|整体完全成功率为5.6%（规则判定）/5.3%（AI语义判定），两种判定器交叉验证结果一致]]（24:08）。[[prompt-injection-attack|prompt injection 无法靠打补丁彻底修复]]，因为读取并服从文本指令正是语言模型的核心工作机制（21:08, 24:08）。这套测评之所以能做起来，靠的正是 [[trajectory-log-enables-large-scale-evaluation|轨迹日志把 AI 每步操作完整记录下来]]，否则无法逐条判定攻击是否成功（33:14）。

### 默认配置与防护建议

默认新会话是 [[deepseek-harness-workspace-write-default|workspace-write]]，AI 只能改指定项目文件夹（24:08, 27:11）。默认不装 [[deepseek-harness-default-no-web-fetch|web fetch]] 工具（24:08）；[[deepseek-harness-web-search-tool|web search 默认开启，返回摘要而非原页面，注入面较小]]，而 [[deepseek-harness-web-fetch-tool|web fetch 把整页原始内容喂给 AI]]，且 [[web-fetch-ssrf-risk|没有内网防控，可能被诱导访问内网服务（SSRF）]]，建议先确认机器是否能访问内网敏感服务，能访问则不要装（27:11）。处理不可信内容应切到 [[deepseek-harness-read-only-mode|read-only 模式]]，但要注意 [[deepseek-harness-read-only-limitation|该模式只拦写不拦读]]，SSH 私钥等仍可被读出并外传（09:04, 27:11）。[[deepseek-harness-full-bypass-mode|完全放开模式]]相当于撤掉所有权限控制，不应轻易启动（27:11）。远程访问管理界面应走 [[ssh-tunnel-secure-remote-access|SSH 隧道]]而非直接暴露端口（24:08）。密钥文件权限过松需用 [[unix-file-permission-600|chmod 600]] 修正，但 [[file-permission-chmod600-ai-bypass|文件权限挡不住 AI 本身，因为 AI 以用户身份运行拥有用户全部权限]]（06:02, 27:11）；[[dsh-hidden-config-folder|.dsh 隐藏文件夹]]存放密钥配置和日志，[[dsh-folder-backup-caution|不应同步网盘或提交代码仓库]]（27:11）。密钥泄露风险还体现在存储层面：[[credentials-yaml-plaintext-storage|credentials.yaml 界面显示打码，磁盘上其实是明文]]（06:02）。数据外传风险方面，[[deepseek-harness-data-offsite-risk|本地文件一旦被 AI 读取就要传到远端服务器处理]]，联想到 [[samsung-chatgpt-leak-incident|三星员工贴源码到 ChatGPT 后被全公司禁用生成式 AI]]的教训（03:00）；[[workspace-secrets-exfiltration-risk|密钥密码证件类文件不应放入工作区]]（06:02）。此外还存在 [[deepseek-harness-anonymous-id-mechanism|匿名 ID 长期追踪]]问题：一旦某次对话出现真实信息就会 [[anonymous-id-deanonymization|导致整份历史使用档案被去匿名化]]，且[[anonymous-id-reset-history-persistence|删除 ID 文件重置后旧记录仍挂在旧编号下]]，不过这属于 [[vendor-documented-not-classified-as-vulnerability|官方文档已写明的设计行为，未被计入漏洞库]]（06:02）。

### 插件生态：审查与投毒风险

[[deepseek-harness-plugin-ecosystem-growth|带插件标签的仓库13天内从288个涨到超1万个]]，但 [[no-official-plugin-marketplace-review|没有官方市场审核]]，[[plugin-code-equivalent-risk|插件能做的事和普通代码完全一样，唯一区别是用户不知道它具体做了什么]]（30:12）。审查流程：先用 [[npm-publisher-audit|npm view 查发布者、仓库、维护者]]，看 [[publisher-trust-signals|历史记录和 star 增长是否自然]]；再用 [[npm-pack-safe-inspection|npm pack 下载不触发安装脚本]]，解压后用 [[grep-dangerous-keywords-plugin-review|grep 搜索 child_process/spawn/fetch/.ssh/credential/process.env]] 等危险关键词；最后用 [[npm-ls-dependency-audit|npm ls --all 检查完整依赖链]]，留意 [[dependency-count-anomaly-signal|依赖数量异常]]和 [[typosquatting-dependency-risk|拼写投毒]]（如把 request 改成 requests，即 [[typosquatting-plugin-name-deception|字母投毒手法]]）（30:12, 33:14）。朱雀测评显示 [[prompt-injection-attack|安装带恶意指令的 skill 插件，注入成功率14%-16%]]（30:12）。即便插件自称是安全类插件也要 [[security-labeled-plugin-scrutiny|同样审查不能免检]]，例如 [[corrector-npm-package-case|corrector 这个包并无独立评测验证其安全能力，宣传更像蹭热度营销]]（33:14）。原则是 [[plugin-dependency-comprehension-principle|看不懂就不装，弃用成本远低于中招后重装系统的代价]]（33:14）。

### 事件响应与行业背景

若怀疑遭遇攻击，应 [[incident-response-timeline-localization|先定位大致时间点]]，再用 [[grep-trajectory-log-keyword-search|grep 搜索轨迹日志中的 cordis define/run 和 subprocess 关键词]]，命中即说明攻击链被走通（33:14）。可以用 [[grep-periodic-monitoring|定期跑 grep 当报警器]]，或用 [[inotifywait-log-monitoring|inotifywait 监听日志文件自动触发检查]]（33:14）。行业层面，[[deepseek-codex-harness-open-source-timeline|DeepSeek 8月13日开源 harness，8天后 OpenAI 也开源了 Codex harness（Apache 2.0 协议）]]，标志着 [[agent-harness-open-source-race-stage|agent 运行框架进入"谁先开放谁先站位"的阶段]]，同时也意味着 [[security-talent-value-with-framework-popularity|随框架普及，安全人才价值也水涨船高]]（36:16）。总体 [[agent-harness-security-hardening-checklist|加固建议]]：端口不暴露公网、沙箱权限收紧、避免随意抓取网页、密钥敏感路径不外泄、配合日志告警监控（36:16）。

## 值得记住的细节

- [00:00] 安装只需一条命令，自动打开本机3080端口界面；未选工作区前聊天框锁定不可用。
- [06:02] YAML `!!js` 标签是第一个漏洞（配置加载任意代码执行）的利用切入点。
- [06:02] credentials.yaml 界面打码但磁盘明文存储密钥。
- [15:05] 管理接口暴露60多个功能，代码中留有"权限功能待实现"的 TODO。
- [15:05] 第五个漏洞 CVSS 9.8 分，影响 0.11 rc2 版本，截至8月24日发稿时修复情况仍无定论。
- [18:07] 判断请求是否本机的依据仅是可伪造的 HTTP Host 字段是否等于 localhost。
- [18:07] dsh2 shell 利用脚本8月20日上线，一条命令完成攻击，还能批量扫描全网暴露服务。
- [21:08] 从公开到奇安信定级9.8分中间隔了10天。
- [21:08] 腾讯朱雀实验室14,560次测试：信息泄露成功率35.7%，写操作调用成功率仅2.5%。
- [21:08] 纯文本注入455次测试成功率0%；藏进PDF元数据/表格/零宽字符后成功率升至25.5%（116次成功）。
- [24:08] 综合14000多处组合测试整体完全成功率5.6%（规则判定）/5.3%（AI判定）。
- [27:11] .dsh 隐藏文件夹用 `ls -a` 查看；密钥文件权限过松用 `chmod 600` 修正。
- [27:11] read-only 模式只拦写不拦读，SSH 私钥仍可被读出外传。
- [30:12] 插件仓库13天内从288个涨到超1万个，增幅超40倍。
- [30:12] 审查命令三件套：`npm view 插件名 repository homepage maintainers`、`npm pack 插件名`、`npm ls --all`。
- [30:12] 朱雀测评：安装带恶意指令的 skill 插件，注入成功率14%-16%。
- [33:14] 轨迹日志存放在 .dsh 文件夹下，append-only 无法被篡改删除。
- [36:16] DeepSeek 8月13日开源 harness，OpenAI 8天后开源 Codex harness（Apache 2.0）。

## 这个视频适合谁 / 可以跳过什么

适合：正在使用或考虑部署 DeepSeek Harness 的开发者、需要评估 agent 框架安全风险的安全从业者、关注 prompt injection 和沙箱逃逸机制的技术人员。

可以跳过：如果只想知道"现在能不能用"，可直接看"默认配置与防护建议"和"加固建议"部分（24:08起及36:16），不必细究每个漏洞的具体利用代码实现细节（09:04-15:05 的技术链路对非安全背景观众可选择性跳过）。
