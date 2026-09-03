---
video_id: WrwA7FYGPdQ
url: https://www.youtube.com/watch?v=WrwA7FYGPdQ
title: DeepSeek Harness 开源 11 天爆 5 个漏洞：AI 读网页电脑被控，有人 API 额度已被盗刷 | QVD-2026-57410 CVSS9.
channel: 网络小白_Uncle城
published: '2026-09-02'
duration: '37:08'
transcript_origin: whisper
tags:
- video
---

# DeepSeek Harness 开源 11 天爆 5 个漏洞：AI 读网页电脑被控，有人 API 额度已被盗刷 | QVD-2026-57410 CVSS9.

摘要: [[2026-09-02-deepseek-harness-开源-11-天爆-5-个漏洞ai-读网页电脑被控有人-api-额度-summary|完整摘要]]

## 知识点

- [[agent-definition]] — 只能进行文字问答、除了回复文字之外无法执行其他动作的 AI 称为 chatbot；而套上 harness 后能读取文件、修改代码、执行命令行并调用外部工具的 AI，才被称为 agent。（[00:00](https://youtu.be/WrwA7FYGPdQ?t=0)）
- [[agent-harness-open-source-race-stage]] — DeepSeek 与 OpenAI 相继开源各自的 agent harness，标志着 agent 运行框架正式进入了「谁先开放谁先站位」的阶段。（[36:16](https://youtu.be/WrwA7FYGPdQ?t=2176)）
- [[agent-harness-security-hardening-checklist]] — 针对 agent harness 的安全加固建议包括：端口不暴露在公网、sandbox权限收紧、避免随意抓取网页内容、确保密钥与敏感路径不外泄，并配合日志告警监控，可以把已知风险压到较低水平。（[36:16](https://youtu.be/WrwA7FYGPdQ?t=2176)）
- [[agent-model-harness-formula]] — DeepSeek 官方提出 agent 等于 model 加 harness 的公式：model 负责理解语言、做决策、生成回复；harness 负责把 model 的决策转化为文件读写、代码修改、命令执行等实际操作。（[00:00](https://youtu.be/WrwA7FYGPdQ?t=0)）
- [[agent-vs-chatbot-autonomous-file-access]] — 相比聊天框「你发什么就是什么」的可控输入方式，agent 会自主决定去读取什么文件、上传什么文件，这使得数据泄露风险比普通 chatbot 更难预判和控制。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- [[agentic-write-actions]] — 测评方准备了8个模拟敏感工具，用注入指令诱导AI真正调用这些工具执行操作的攻击测试，成功率仅为2.5%。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- [[ai-code-as-temporary-plugin]] — 在 DeepSeek Harness 框架里，AI 可以自己写代码并把它注射成临时插件运行，这意味着安装一个插件本质上就是往 Harness 里添加一段可执行代码。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[anonymous-id-deanonymization]] — 只要某次对话中出现过一次真实信息（比如贴过带公司邮箱的代码，或提到过真实姓名），挂在该匿名 ID 下的整份使用档案就会立刻与真人对应上，从匿名变成实名。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[anonymous-id-reset-history-persistence]] — 删除本机保存匿名 ID 的文件后，下次启动 Harness 会生成一串全新的 ID，但换新之前的历史使用记录仍然挂在旧的编号下面，不会随之消失。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[apache-2-0-license]] — OpenAI 开源 Codex harness 采用的是 Apache 2.0 协议，允许任何人自由使用、修改和分发该代码。（[36:16](https://youtu.be/WrwA7FYGPdQ?t=2176)）
- [[attack-bypasses-api-key]] — 整个攻击过程中，攻击者从未使用过受害者的 DeepSeek API 密钥；他直接控制的是 DeepSeek Harness 该调用哪个模型、执行什么命令，密钥完全被绕过。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
- [[chained-sandbox-escape-rce-vuln]] — 第四个漏洞是把前面几个漏洞串联组合而成的链式沙箱逃逸，最终导致远程命令执行（RCE）。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[config-file-backdoor-persistence]] — 攻击者拿到命令执行权限后可以改写配置文件、埋入恶意代码，之后每次启动 DeepSeek Harness 加载配置时这段代码都会执行，重启电脑无法清除，只要配置文件存在后门就一直存在。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
- [[context-object-security-bypass]] — DeepSeek Harness 的权限检查逻辑被安放在服务调用路径的半路而非入口处，插件正常走接口调用服务时会被检查，但直接窃取整个上下文对象绕开该路径就不会被拦截。（[12:04](https://youtu.be/WrwA7FYGPdQ?t=724)）
- [[cordis-define-run-plugin-api]] — DeepSeek Harness 中的 AI 可以在线写一段代码、注射成临时插件马上运行，这是官方功能，插件定义接口叫 Cordis Define、运行时接口叫 Cordis Run，框架的核心卖点正是让 AI 能给自己在线写工具。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
- [[corrector-npm-package-case]] — corrector 这个包确实存在，但没有任何独立评测能验证其自称的安全验证能力，其宣传很大程度上是蹭朱雀论文热度的营销行为。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[credentials-yaml-plaintext-storage]] — API 密钥保存在 credentials.yaml 文件中，界面显示的是打码后的描述符，但磁盘上该文件保存的其实是未加密的明文密钥，打开文件即可直接看到。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[cvss-severity-score]] — 第五个漏洞的 CVSS 评分高达 9.8 分，是本系列已披露漏洞中评分最高的一个，影响版本为最新的 0.11 rc2。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
- [[deepseek-codex-harness-open-source-timeline]] — DeepSeek 于8月13号开源了自己的 agent harness，8天之后 OpenAI 也开源了 Codex harness。（[36:16](https://youtu.be/WrwA7FYGPdQ?t=2176)）
- [[deepseek-harness]] — DeepSeek Harness 上线仅一天 GitHub star 数就突破7万，但在短短11天内被曝出5个安全漏洞。（[00:00](https://youtu.be/WrwA7FYGPdQ?t=0)）
- [[deepseek-harness-anonymous-id-mechanism]] — 首次用自己申请的 API 密钥连接服务器验证成功后，Harness 会在本机生成一串随机的匿名 ID，单看一条请求无法确认使用者身份，但该 ID 是稳定不变的，服务器会看到同一编号发起的所有请求。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[deepseek-harness-approval-fail-close]] — 审批机制遵循 fail-close 原则，即审批流程出现异常或超时无响应时默认拒绝执行，而不是默认放行。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- [[deepseek-harness-batch-script-mode]] — 该模式通过让模型编写脚本一次性完成多步工具调用，减少多轮交互带来的 token 消耗。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- [[deepseek-harness-chained-sandbox-escape-rce]] — 该链式漏洞本身没有产生新的攻击面，而是把前面三个漏洞串联起来，使原本运行在 VM 沙箱里的插件能够直接在主机上执行命令，达成远程命令执行（RCE），性质上比前三个孤立的单点问题更严重。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
- [[deepseek-harness-config-code-execution]] — DeepSeek Harness 解析配置文件时，会把某个值当作 JavaScript 代码在加载配置的那一刻直接执行，验证者在配置文件中隐藏一行写文件代码即可让其在 Harness 启动加载配置时立即运行。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
- [[deepseek-harness-creative-mode]] — 创造模式允许 AI 在任务执行过程中动态生成新工具并立即加载调用，而非局限于预先定义好的工具集合。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- [[deepseek-harness-cve-2026-57410]] — DeepSeek Harness 开源当天即被曝出4个漏洞（其中2个等级为严重），8月24号又被曝出第5个漏洞，等级为极危，CVSS 评分达到9.8分，是该框架已知漏洞中评分最高、最严重的一个。（[00:00](https://youtu.be/WrwA7FYGPdQ?t=0)）
- [[deepseek-harness-data-offsite-risk]] — 只要用户在 Harness 上让 AI 读取本地文件，该文件内容就必须经网络传输到 DeepSeek 服务器由远端模型处理后再返回结果，数据一旦离开本机就只能依赖对方的服务条款承诺，出问题也无法自行审计。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- [[deepseek-harness-day-one-vulnerability-disclosure]] — DeepSeek Harness 开源的当天，一位独立安全研究员就发布了评审报告，一次性披露4个漏洞，且官方安全库当天就全部收录并验证了这些漏洞。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[deepseek-harness-default-localhost-only]] — DeepSeek Harness 的 web 服务默认只监听本机局域网地址，能挡住局域网内其他设备的连接，但挡不住同一台电脑上的其他程序访问，这个默认值并不绝对安全。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
- [[deepseek-harness-default-no-web-fetch]] — DeepSeek Harness 官方出厂默认不安装抓取网页的工具，需要用户主动安装才能使用，这在一定程度上降低了被动读取恶意网页内容的风险。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
- [[deepseek-harness-default-workspace-writable]] — DeepSeek Harness 开启新会话的默认权限是工作区可写（workspace-writable），AI只能改动用户指定的项目文件夹，无法越权修改其他区域文件。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
- [[deepseek-harness-everything-is-plugin]] — DeepSeek Harness 秉持「一切皆插件」的设计理念，就连界面本身也是以插件形式存在的。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[deepseek-harness-exploit-chain]] — 利用链第一步：攻击者调用 DeepSeek Harness 内部接口注册一个假的模型提供者，服务地址指向攻击者自己的服务器；这个模型是假的，不会做任何推理，只会按攻击者预设内容返回结果。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
- [[deepseek-harness-exposure-methods]] — 该漏洞被远程利用的前提是管理接口被暴露到公网，典型方式有两种：一是在云服务器上部署 DeepSeek Harness 并做端口映射、把管理端口直接暴露到公网；二是挂反向代理再配上域名，同样会暴露整套管理接口；这两类部署只要攻击者知道地址就能远程接管。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
- [[deepseek-harness-full-bypass-mode]] — 完全放开模式下 AI 做任何操作都不会询问用户，启动这一档相当于撤掉所有权限控制，对应攻击链第三步「滥用运行插件的接口」，各类高危操作（如删除整个系统、删除磁盘）都可能由此模式引发，不应轻易启动。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
- [[deepseek-harness-injection-success-rate]] — 研究团队把所有能测的攻击入口、隐藏方式和攻击方法组合全部测了一遍，共约14000多处，测得整体完全成功率为5.6%，即每100次攻击中约有5-6次完全得手。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
- [[deepseek-harness-loopback-binding-limitation]] — DeepSeek Harness 默认只监听本机回环地址 127.0.0.1，外部设备无法直接连入，能挡住远程攻击，但接口缺乏认证的问题依然存在：同一台电脑上任何能向该端口发起 HTTP 请求的程序（不明软件、潜伏的木马、浏览器诱导安装的恶意脚本等）都能利用这个漏洞。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
- [[deepseek-harness-management-api-exposure]] — DeepSeek Harness 的管理入口（浏览器操作界面底层所走的接口）一共暴露了 60 多个功能，其中一批属于高权限功能，正常设计上应只有框架自己能调用。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
- [[deepseek-harness-management-port-config]] — DeepSeek Harness 的管理界面默认只监听本机回环地址127.0.0.1的3080端口，在此状态下外部设备根本连接不上，此前提到的远程打法在默认配置下走不通。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
- [[deepseek-harness-mechanical-mode]] — 机械模式限定 agent 只能使用命令行和文件编辑两种工具，主要用于跑分测试场景。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- [[deepseek-harness-modes]] — DeepSeek Harness 界面提供四种运行模式，其中标准模式会开启全部功能，PTC 模式（全程序可编程工具调用）更适合日常写代码场景使用。（[00:00](https://youtu.be/WrwA7FYGPdQ?t=0)）
- [[deepseek-harness-partial-isolation-reporting]] — 若操作系统隔离机制未能完全拦截，DeepSeek Harness 会明确上报当前隔离状态为部分生效，让用户了解实际防护程度。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- [[deepseek-harness-permission-tiers]] — DeepSeek Harness 的权限自分为三档，分别是只读工作区、工作区可写和完全放开，用户可根据需要在这三档之间切换配置。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
- [[deepseek-harness-plugin-architecture]] — DeepSeek Harness 中模型、工具、沙箱（sandbox）、网页界面，甚至决定 agent 下一步行为的主循环核心逻辑本身都是可插拔的插件，理论上可以整体替换重启。（[00:00](https://youtu.be/WrwA7FYGPdQ?t=0)）
- [[deepseek-harness-plugin-ecosystem-growth]] — 带 subscribe-sh-plugin 标签的 DeepSeek Harness 插件仓库数量从第一天的 288 个，13 天内涨到超过 1 万个，增幅超过 40 倍。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[deepseek-harness-port-exposure-risks]] — 把 DeepSeek Harness 部署在云服务器上并做端口映射、将3080端口转发到公网，是导致无认证后台被暴露到公网的常见风险操作之一。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
- [[deepseek-harness-rce-vulnerability]] — DeepSeek Harness 曝出的漏洞中包含远程命令执行（RCE）漏洞，且相关的最新代码漏洞利用代码均已公开。（[36:16](https://youtu.be/WrwA7FYGPdQ?t=2176)）
- [[deepseek-harness-read-only-limitation]] — read-only 模式只拦截写入而不拦截读取，AI 依然能读取机器上的文件，包括本地存储的密钥。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
- [[deepseek-harness-read-only-mode]] — 处理不可信内容（如从网上下载的陌生仓库、外部文档）时应先切到 read-only 模式，最新版 DeepSeek Harness 中输入 permission read only 即可切换，切换后沙箱和审批策略会一并切换。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
- [[deepseek-harness-readonly-mode-read-leak]] — 很多人处理不可信项目时会切换到只读模式、认为这样就安全，但验证发现只读模式下 AI 写文件会被文件系统权限拒绝，读取工作区外的文件（如 SSH 私钥、保存密码密钥的环境变量）却能成功，且读到的内容还可以被发送到外部服务器，说明只读模式不限制查看权限。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
- [[deepseek-harness-replay-branch-debugging]] — 相比其他 agent 出事后只能靠猜测或依赖有限上下文分析报错，DeepSeek Harness 能像回放录像一样完整重现整个交互过程，并支持从任意节点分支重跑对比不同选择的结果。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- [[deepseek-harness-same-machine-vuln-no-fix]] — 同一台电脑上的其他恶意程序能够无认证访问 DeepSeek Harness 接口，这是框架自身的设计问题，配置层面没有开关能够关掉，目前唯一的应对办法是不要安装来路不明的软件。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
- [[deepseek-harness-sandbox-os-implementation]] — 三层沙箱的底层实现按操作系统区分，分别调用 Linux、macOS、Windows 各自系统自带的隔离机制，而非自行重新造轮子。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- [[deepseek-harness-setup]] — 安装 DeepSeek Harness 只需先装好 Node.js，随后执行一条命令即可自动打开本机3080端口对应的网页界面；首次使用需在设置中配置 API 密钥并选择工作区，配置完成后无需重启即可直接使用。（[00:00](https://youtu.be/WrwA7FYGPdQ?t=0)）
- [[deepseek-harness-three-tier-sandbox]] — 三层沙箱默认选项是工作区可写，即 AI 只能修改用户指定工作文件夹内的内容；只读档只能查看文件不能修改；完全放开档可访问电脑上所有文件，切换该模式时需要二次确认。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- [[deepseek-harness-tool-call-command-execution]] — 利用链第二、三步：攻击者触发一次新的对话让 DeepSeek Harness 连接假模型，随后假模型以工具调用指令的形式先创建对话再下发任务，任务内容是运行一条命令，DeepSeek Harness 按指令调用命令行工具，在受害者机器上以受害者账户权限执行攻击者指定的命令。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
- [[deepseek-harness-trajectory-log]] — 轨迹日志采用 append-only 特性，只能往里追加内容而不能修改或删除已写入的记录，确保模型历史行为可完整追溯。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- [[deepseek-harness-unauthenticated-management-api]] — DeepSeek Harness 的管理接口完全没有认证机制，不需要账号、密码或令牌；官方文档也承认加密和认证不在第一版范围内，第一版威胁模型只考虑恶意网页这一种攻击场景。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
- [[deepseek-harness-vm-sandbox]] — 该沙箱是在 Harness 插件代码所运行的 Node.js 进程内部划出一块隔离区域，让不可信任的代码（如插件代码）在其中运行而不能触及外部，设计上插件不能直接访问主机，只能通过指定接口调用宿主服务。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
- [[deepseek-harness-vuln-disclosure-timeline]] — 早在 8 月 14 号，已有研究者在 GitHub 上公开讨论并发布了一份审计，把这个管理接口没有认证的问题完整讲了一遍，连修复建议都写好了，但当时项目还没有响应处理。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
- [[deepseek-harness-vulnerability-disclosure]] — DeepSeek Harness 开源当天就被曝出4个漏洞，其中2个被评定为严重（severe）级别，8月24号最新代码又新增第5个严重漏洞。（[36:16](https://youtu.be/WrwA7FYGPdQ?t=2176)）
- [[deepseek-harness-vulnerability-disclosure-gap]] — 该漏洞报告因平台缺少私密的漏洞上报通道，研究者只能选择公开贴出报告，报告发布后一直没有人修复。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- [[deepseek-harness-vulnerability-severity-levels]] — 本次公开的4个漏洞中，前两个的危险等级是高危，后两个是严重，而严重是漏洞危险等级表上最顶端的一档。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[deepseek-harness-web-fetch-tool]] — web fetch 是让 AI 把任意网页完整内容全部拉取下来读取的工具，官方出厂不会安装，必须手动修改配置文件才能启用。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
- [[deepseek-harness-web-search-tool]] — web search 是 DeepSeek Harness 默认开启的搜索工具，返回结果是摘要而非原始网页内容，注入面相对较小。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
- [[deepseek-harness-workspace-scope]] — DeepSeek Harness 的工作区（workspace）是用户指定给 AI 操作的文件夹，AI 只能在该文件夹范围内活动；未选定工作区之前，聊天输入框会处于锁定状态无法使用。（[00:00](https://youtu.be/WrwA7FYGPdQ?t=0)）
- [[deepseek-harness-workspace-write-default]] — DeepSeek Harness 默认是 workspace-write 模式，AI 要改文件、跑命令只能在指定的项目文件夹里进行，其他地方只能看不能改。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
- [[dependency-count-anomaly-signal]] — 审查依赖列表时若发现一个功能简单的插件背后拖了几十甚至上百个依赖包，这是不正常的信号，需要警惕。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[docker-sandbox-info-leak-vuln]] — 第二个漏洞是「Docker 沙箱信息泄露」，即运行在 Docker 沙箱中的代码执行环境存在敏感信息被泄露出去的问题。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[dsh-api-key-file-permission]] — DeepSeek API 密钥存放在 .dsh 文件夹内的一个文件中，DeepSeek Harness 启动时会自动检查该文件权限，权限过松会报错并提示收紧，可用 chmod 600（修改文件权限的命令）来修正。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
- [[dsh-folder-backup-caution]] — .dsh 文件夹不应同步到网盘、云备份，也不应提交到代码仓库，因为里面含有 API 密钥等敏感信息；出问题时可以到该文件夹查轨迹日志排查。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
- [[dsh-hidden-config-folder]] — DeepSeek Harness 的密钥、配置、运行轨迹和日志都保存在用户主目录下的隐藏文件夹 .dsh 中，可用 ls -a 命令（列出包含隐藏文件的目录内容）查看其中文件清单。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
- [[dsh2-shell-exploit-tool]] — 该漏洞已有现成的开源利用脚本 dsh2 shell，一条命令就能完成整个攻击，自带假模型服务器无需准备真实模型，还提供批量扫描模式可自动搜索全网暴露此漏洞的 DeepSeek Harness 服务，攻击者无需懂原理即可使用。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
- [[dsh2-shell-vulnerability-weaponization]] — DSH2 Shell于8月20日上线，使得该漏洞被工具化，具备了可被自动利用的能力。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- [[execute-agent-context-leak]] — 动态加载的插件（程序运行过程中临时装入的插件）被直接传入名为 Execute Agent Context 的上下文对象，该对象存放着宿主程序运行时的各种服务引用和状态，且没有经过沙箱隔离或检查。（[09:04](https://youtu.be/WrwA7FYGPdQ?t=544)）
- [[file-permission-chmod600-ai-bypass]] — 官方文档说明文件权限设置能挡住同一台电脑上的其他用户，但挡不住 AI 本身，因为 AI 运行时使用的是用户自己的身份，拥有用户所有的权限。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[grep-dangerous-keywords-plugin-review]] — 解压插件包后用 grep 搜索 child_process 和 spawn（启动子进程，是攻击链拿到执行能力的最后一步）、fetch（发网络请求，用于数据外传）、.ssh（密钥目录）、credential（凭证字段）、process.env（读环境变量，密钥常存于此），命中哪条就翻到对应代码看它具体在干什么。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[grep-periodic-monitoring]] — 这条grep敏感关键词的命令平时也可以当报警器用，隔一阵子跑一遍，一旦发现命中就说明有攻击事件发生。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[grep-trajectory-log-keyword-search]] — 用grep搜索轨迹日志里的关键词（如插件定义接口、插件运行接口和subprocess）三个敏感调用，一旦命中说明很可能有人在机器里走通了从注入到执行的完整攻击链。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[harness-rapid-iteration-security-instability]] — 从该漏洞的处置过程可以看出，DeepSeek Harness这类框架仍处于快速施工期，安全边界可以说是一天一个大变样。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- [[hidden-injection-payload-location]] — 测试对比发现，恶意指令若直接写在文档正文等普通文本中让AI读取，455次测试成功率为0%，全部被防住。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- [[hidden-text-prompt-injection-technique]] — 人类正常浏览网页很少会打开开发者工具查看源码，而 AI 读取网页本质就是读取源码，因此隐藏在源码或元数据中的提示注入指令对人不可见、对 AI 却完全可见。（[12:04](https://youtu.be/WrwA7FYGPdQ?t=724)）
- [[host-header-localhost-check-bypass]] — DeepSeek Harness 判断某个高权限请求是否来自本机的依据，是检查该 HTTP 请求头中 Host 字段的值是否等于 localhost，而 Host 字段是每个 HTTP 请求都携带、可被伪造的信息。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
- [[host-header-spoofing-localhost-bypass]] — DeepSeek Harness 通过检查请求的 host 字段是否为 localhost 来判断请求是否来自本机，但 host 字段完全由客户端填写，攻击者从外网发起请求并把 host 改成 localhost，即可让服务端把外部请求当成本机请求处理，导致本机检查完全失效。（[18:07](https://youtu.be/WrwA7FYGPdQ?t=1087)）
- [[incident-response-timeline-localization]] — 如果真的遭遇攻击，第一步应该先定位大致时间点，回忆大概是什么时候让AI读取了那个可疑文件。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[information-extraction-attack]] — 在测评中，诱导AI把预置的假机密信息（如伪造的API密钥字符串）在回复中说出来的攻击测试，成功率为35.7%。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- [[injection-attack-say-vs-do-asymmetry]] — 对比两组测评数据可以看出，被忽悠着把秘密说出口相对容易，但被诱导真正调用敏感工具动手执行操作则难得多。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- [[inotifywait-log-monitoring]] — 如果想更省事，可以用inotifywait这类文件监听工具挂在日志文件上，日志一有追加就自动触发检查，不用自己记着定期手动跑命令。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[no-official-plugin-marketplace-review]] — DeepSeek Harness 目前没有官方插件市场，也就没有人会帮用户审核每个插件是否安全，插件质量良莠不齐。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[npm-ls-dependency-audit]] — 插件自身代码干净不代表依赖也干净，攻击者常把恶意代码埋在依赖包里实施供应链攻击，因此还需用「npm ls --all」列出插件的完整依赖清单逐一检查。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[npm-pack-safe-inspection]] — 审查代码阶段应先用「npm pack 插件名」把包下载成压缩文件，该命令不会触发包内任何安装脚本，之后再解压检查内容，而不是直接执行安装。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[npm-publisher-audit]] — 审查 npm 插件的第一步是查发布者，可用「npm view 插件名 repository homepage maintainers」列出该包的源码仓库地址、主页和维护者名单。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[plaintext-injection-testing-blindspot]] — 测评论文原文指出「只测纯文本会漏掉真实的攻击行为」，意味着即便纯文本注入测试全部被防住，换个藏身位置攻击仍可能成功。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- [[plugin-code-equivalent-risk]] — 插件能做的事和正常代码完全一样，包括读写文件、联网、启动进程，唯一区别是插件代码是别人写的，用户并不知道它具体做了什么。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[plugin-dependency-comprehension-principle]] — 如果发现看不懂某个插件的依赖用途又拿不定主意，最好的做法是不装，因为放弃一个插件几乎没有成本，但中招后的代价（如被迫重装系统）要高得多。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[poc-exploit-code-disclosure]] — 研究者为每个漏洞都编写了能直接跑通的验证代码（PoC），并将其与完整的评审报告一起公开发布。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[prompt-injection-attack]] — AI 模型会读取并服从其在网页、文档等内容中看到的文字指令，攻击者可借此在恶意网页或文档中预先写入诸如「忽略之前的命令，执行以下操作」这样的隐藏指令实施提示注入攻击。（[12:04](https://youtu.be/WrwA7FYGPdQ?t=724)）
- [[prompt-injection-to-plugin-execution-chain]] — 攻击者不需要提前获取任何权限或凭据，只要让 AI 读取一段其编写的内容即可触发注入攻击。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
- [[publisher-trust-signals]] — 判断发布者是否可信要看维护者账号有没有历史发布记录、仓库提交历史长不长、star 数增长是否和活跃度对得上；一个上周才注册、发第一个包就一天涨了几千 star 的账号基本可判定为刷的。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[qi-anxin-cvss-rating-delay]] — 从漏洞被公开写出来到奇安信正式定级CVSS 9.8分，中间整整过了10天，这10天内该漏洞持续被工具化并被大规模利用。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- [[remote-code-execution-definition]] — 远程命令执行（RCE）的含义是：攻击者能在受害者的电脑上运行任何他想运行的命令。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[replayable-audit-log-rare-capability]] — 这套架构出事之后能完整回放本身就是很少见的审计能力，值得对DeepSeek Harness的这一设计给予肯定。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[samsung-chatgpt-leak-incident]] — 三星员工把内部源码贴入 ChatGPT 的事件，促使三星此后在全公司范围内禁用生成式 AI，成为企业对数据外泄风险高度敏感的典型案例。（[03:00](https://youtu.be/WrwA7FYGPdQ?t=180)）
- [[security-labeled-plugin-scrutiny]] — 即使一个插件自称是做安全防护的，也不能因此就默认信任、跳过审查，没有任何插件是例外。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[security-talent-value-with-framework-popularity]] — 随着 agent harness 框架越来越普及，能做安全检查的人才价值也会随之越来越高。（[36:16](https://youtu.be/WrwA7FYGPdQ?t=2176)）
- [[ssh-tunnel-secure-remote-access]] — 若确实需要远程访问 DeepSeek Harness 管理界面，推荐做法是走 SSH 隧道：在自己电脑上发起加密连接，把远程3080端口映射回本地使用，而不直接把端口暴露到公网。（[24:08](https://youtu.be/WrwA7FYGPdQ?t=1448)）
- [[subprocess-service-host-privilege-escalation]] — PoC 让沙箱内插件调用窃取到的 subprocess 服务的 spawn 方法，在主机上成功写入文件并输出「unconfined host process」，证明命令逃逸出沙箱、在主机上以用户权限执行成功。（[12:04](https://youtu.be/WrwA7FYGPdQ?t=724)）
- [[tencent-zhuque-lab-security-assessment]] — 腾讯朱雀实验室拿这套Harness框架做过一次安全测评，一共跑了14,560次真实测试。（[21:08](https://youtu.be/WrwA7FYGPdQ?t=1268)）
- [[todo-placeholder-security-gap]] — DeepSeek Harness 工具执行模块的代码中留有一条 TODO，内容为‘权限功能待实现’，说明拦截高危操作的权限功能官方自己都还没写完。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
- [[trajectory-log-append-only]] — 轨迹日志只能追加新记录，已写入的记录无法被修改或删除，即使攻击者拿到了命令执行权限、想删除记录消灭证据也做不到，因为日志本身具有防篡改性。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[trajectory-log-enables-large-scale-evaluation]] — DeepSeek Harness的14000多次安全测评之所以能做起来，靠的正是这套轨迹日志：测试中AI每一步操作都被完整记录，测评程序才能回头逐条检查攻击是否成功，如果没有这套日志，测试结果根本无法判定。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[trajectory-log-replay-diagnosis]] — 对比正常绘话与遭受注入后绘话的轨迹日志回放，可以精确看到第几轮读取了恶意文件、读回来了什么内容，以及模型从哪一步开始出现异常行为，注入的生效点一目了然。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[trajectory-log-storage-location]] — 轨迹日志文件保存在 .dsh 文件夹下，也就是此前提到的插件相关数据的落点位置。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[typosquatting-dependency-risk]] — 审查依赖列表要留意是否混有拼写奇怪、与知名包名只差一两个字母的依赖包，这类高度可疑的包是供应链投毒常用的伪装手法。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[typosquatting-plugin-name-deception]] — 常见的插件投毒手法之一是在合法包名基础上多写一个字母（如把 request 改成 requests）来欺骗粗心用户安装恶意插件。（[33:14](https://youtu.be/WrwA7FYGPdQ?t=1994)）
- [[unix-file-permission-600]] — 把文件权限设为 600 意味着该文件仅创建者本人可读写，系统内其他用户都打不开。（[30:12](https://youtu.be/WrwA7FYGPdQ?t=1812)）
- [[unsafe-subprocess-spawn-no-sandbox]] — 插件跑起来后通过 execute agent context 拿到宿主上下文、取出 subprocess 并用 spawn 在主机上启动进程，该进程权限就是当前登录用户的权限，VM 沙箱、进程沙箱等整条防线都没有参与进来。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
- [[unwired-approval-service-vulnerability]] — 默认配置下，AI 自主调用 cordis define/cordis run 这类高危操作会被直接执行，没有任何审批环节介入。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
- [[vendor-documented-not-classified-as-vulnerability]] — 匿名 ID 长期追踪使用者行为的机制不算作官方漏洞库中的漏洞，因为这是官方自己在模块文档中写明的设计行为，而非未公开的缺陷。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[vm-sandbox-escape-vuln]] — 第三个漏洞是「VM 沙箱逃逸」，即攻击者能够突破虚拟机沙箱的隔离边界逃逸出去。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[vulnerability-chain-composition]] — 文中四个孤立漏洞的共同根因是权限检查被安放在服务调用路径的半路而非调用发生的入口处，单独看每个漏洞都不足为惧，但它们能串成一条完整的攻击链。（[12:04](https://youtu.be/WrwA7FYGPdQ?t=724)）
- [[vulnerability-disclosure-fix-status-tracking]] — 截至作者发稿的8月24日，前述漏洞的修复情况仍未有定论；官方虽发布了 rc7、rc8 直至 0.11 等多个版本，但更新说明中未见明确提到安全修复相关内容。（[15:05](https://youtu.be/WrwA7FYGPdQ?t=905)）
- [[web-fetch-injection-surface]] — web search 只返回结果摘要注入面较小，而 web fetch 把整页所有原始内容原样喂给 AI，网页是别人地盘、内容完全未知，如果确实需要抓取原始网页，应先确认机器是否能访问到内网敏感服务，若能访问则尽量不要安装该工具。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
- [[web-fetch-ssrf-risk]] — web fetch 没有内网防控，机器能访问什么它就能访问什么，例如家里远程连公司内网、云服务器上的内部网络都可能被摸到，这类行为的学名是 SSRF（服务端请求伪造），即诱导工具访问其本不应访问的内网地址。（[27:11](https://youtu.be/WrwA7FYGPdQ?t=1631)）
- [[workspace-secrets-exfiltration-risk]] — 密钥、密码、证件类敏感文件不应放入 AI agent 的工作区，因为 AI 一旦读到这些内容就有可能将其发出去，导致完全脱离用户掌控。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[yaml-config-arbitrary-code-execution-vuln]] — 第一个漏洞是「配置加载任意代码执行」，即通过操纵 Harness 加载的配置文件即可导致任意代码在目标系统上执行。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
- [[yaml-js-tag-syntax]] — Harness 的配置文件是 YAML 格式，而 YAML 支持一种特殊语法，即在值前面写两个感叹号加 js，写成 !!js 这样的标签形式，这正是第一个「配置加载任意代码执行」漏洞的利用切入点。（[06:02](https://youtu.be/WrwA7FYGPdQ?t=362)）
