---
layout: default
title: "Horizon Summary: 2026-02-28 (ZH)"
date: 2026-02-28
lang: zh
---

> From 24 items, 8 important content pieces were selected

---

1. [Anthropic 拒绝五角大楼将 AI 用于大规模监控和自主杀戮的要求](#item-1) ⭐️ 9.0/10
2. [安全专家呼吁开发者停止使用通行密钥加密用户数据](#item-2) ⭐️ 8.0/10
3. [AI 编码怀疑论者尝试使用 AI 智能体将 scikit-learn 移植到 Rust](#item-3) ⭐️ 8.0/10
4. [ChatGPT 周活跃用户近 10 亿，付费订阅用户突破 5000 万](#item-4) ⭐️ 8.0/10
5. [青龙面板遭.fullgc 挖矿木马植入，导致 CPU 占用率达 800%](#item-5) ⭐️ 8.0/10
6. [Google Chrome 默认自动下载 4GB 本地 AI 模型 Gemini Nano](#item-6) ⭐️ 7.0/10
7. [韩国国税厅误曝硬件钱包助记词，导致 480 万美元加密货币被转走](#item-7) ⭐️ 7.0/10
8. [摩托罗拉内部演示文稿泄露，暗示与 GrapheneOS 合作，首款非 Pixel 设备或于 2027 年面世](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic 拒绝五角大楼将 AI 用于大规模监控和自主杀戮的要求](https://notdivided.org/) ⭐️ 9.0/10

人工智能公司 Anthropic 公开拒绝遵守美国战争部（DoW）的新合同条款，这些条款将允许其 AI 模型被用于国内大规模监控和完全自主的致命武器。据报道，这一拒绝导致特朗普政府将 Anthropic 列入黑名单，并命令联邦政府停止使用其技术。 这次对抗为 AI 伦理中的企业责任树立了一个重要先例，直接挑战了政府试图将先进 AI 用于有争议的国内和军事应用的企图。它迫使公众就国家权力的界限、科技公司在国家安全中的作用，以及自主杀戮系统的伦理红线展开辩论。 Anthropic 拒绝的具体要求涉及放宽其 AI 模型的护栏，以允许“任何合法用途”，该公司将此解释为包括国内监控和自主杀戮。相比之下，据报道，OpenAI 已与战争部达成协议，在该部门的机密网络内部署其模型，并声称“不进行国内大规模监控”。

hackernews · BloondAndDoom · Feb 28, 00:54

**背景**: 大型 AI 模型可以显著降低自动化监控的成本并扩大其规模，使大规模监控变得更加可行。自主武器系统（AWS）是可以在没有人工干预的情况下选择和攻击目标的机器，这引发了关于将生死决策权委托给算法的深刻伦理和法律问题。在此背景下提到的美国战争部，可能是对国防部（五角大楼）的一种通俗或历史性指代。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/886082/ai-vs-the-pentagon-killer-robots-mass-surveillance-and-red-lines">AI vs. the Pentagon: killer robots, mass surveillance, and red lines | The Verge</a></li>
<li><a href="https://www.cnbc.com/2026/02/27/trump-anthropic-ai-pentagon.html">Trump admin blacklists Anthropic; AI firm refuses Pentagon demands</a></li>
<li><a href="https://www.hindustantimes.com/world-news/us-news/no-domestic-mass-surveillance-whats-inside-openai-deal-dow-trump-admin-anthropic-ai-tussle-101772250629771.html">'No domestic mass surveillance': What's inside OpenAI's deal with Trump admin amid Anthropic tussle | Hindustan Times</a></li>

</ul>
</details>

**社区讨论**: 社区情绪强烈支持 Anthropic 的立场，但对更广泛的影响深感担忧。主要观点包括：对政府越权和滥用采购规则惩罚“不忠诚”公司的恐惧，对国内监控政策所设定的全球先例的警告，以及对封杀 Anthropic 将损害美国科技生态系统信任的担忧。

**标签**: `#ai-ethics`, `#government-surveillance`, `#autonomous-weapons`, `#corporate-responsibility`, `#national-security`

---

<a id="item-2"></a>
## [安全专家呼吁开发者停止使用通行密钥加密用户数据](https://simonwillison.net/2026/Feb/27/passkeys/#atom-everything) ⭐️ 8.0/10

安全专家 Tim Cappalli 已公开呼吁身份识别行业停止推广和使用通行密钥来加密用户数据。这一警告突出了一个关键风险：当用户不可避免地丢失其通行密钥时，将导致永久性、无法恢复的数据丢失。 这很重要，因为利用 WebAuthn PRF 扩展等功能，使用通行密钥进行客户端加密的趋势日益增长，这造成了大规模数据丢失的系统性风险。遵循此模式的开发者正在构建这样的系统：一旦通行密钥丢失，用户数据将永久无法访问，这错误地应用了通行密钥在身份验证方面的安全优势。 该警告特别针对 WebAuthn 伪随机函数扩展的误用，该扩展允许通行密钥生成确定性的加密密钥。一个关键的注意事项是，与密码不同，通行密钥是设备绑定的加密密钥对，其私钥并非设计为以相同方式进行备份或恢复，这使得密钥丢失对加密数据而言是灾难性的。

rss · Simon Willison · Feb 27, 22:49

**背景**: 通行密钥是一种基于 WebAuthn 标准的无密码身份验证技术，使用公钥密码学。在身份验证过程中，用户的私钥保留在其设备上（如手机或安全密钥），只有公钥与网站共享。WebAuthn PRF 扩展是一项较新的功能，它允许通行密钥也生成一致的加密密钥，一些开发者正将其重新用于客户端数据加密。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bitwarden.com/blog/prf-webauthn-and-its-role-in-passkeys/">PRF WebAuthn and its role in passkeys | Bitwarden</a></li>
<li><a href="https://www.corbado.com/blog/passkeys-prf-webauthn">Passkeys & WebAuthn PRF for End-to-End Encryption (2026)</a></li>
<li><a href="https://bitwarden.com/resources/passkey-vs-password-whats-the-difference/">Passkey vs password: What's the difference? - Bitwarden</a></li>

</ul>
</details>

**标签**: `#security`, `#authentication`, `#passkeys`, `#cryptography`, `#usability`

---

<a id="item-3"></a>
## [AI 编码怀疑论者尝试使用 AI 智能体将 scikit-learn 移植到 Rust](https://simonwillison.net/2026/Feb/27/ai-agent-coding-in-excessive-detail/#atom-everything) ⭐️ 8.0/10

开发者兼 AI 编码怀疑论者 Max Woolf 进行了一项详细的实验，使用 AI 编码智能体从简单任务开始，最终尝试将 Python 的 scikit-learn 机器学习库移植到 Rust，创建了一个暂定名为 'rustlearn' 的项目。该实验测试了 Opus 4.6 和 Codex 5.3 等模型，他发现这些模型比几个月前发布的编码大语言模型好了一个数量级。 该实验展示了 AI 编码智能体在实际能力上的重大飞跃，超越了简单的代码生成，有可能自动化像库移植这样复杂、大规模的软件工程项目。这预示着开发者工作流程可能发生范式转变，AI 智能体可以大幅加速开发周期，并处理那些以前被认为过于耗时的、雄心勃勃的跨语言或跨平台项目。 'rustlearn' 项目的目标不仅是在 Rust 中实现逻辑回归和 k-means 聚类等标准机器学习算法，还要匹配或超越 scikit-learn 实现的性能。作者指出，很难在不听起来像炒作的情况下传达近期模型的巨大改进，因为这些模型持续处理着需要人类开发者数月才能完成的复杂任务。

rss · Simon Willison · Feb 27, 20:43

**背景**: AI 编码智能体是使用大语言模型（LLM）来理解、生成，有时甚至执行基于自然语言指令的代码的自主或半自主软件工具。Scikit-learn 是一个用于机器学习的基础性开源 Python 库，被广泛认为是数据科学的'黄金标准'；它构建在 NumPy 和 SciPy 之上，性能关键部分用 Cython 编写。在 Rust 中，'crate' 是编译和打包的基本单元，相当于其他语言中的库或包，由 Cargo 工具管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Scikit-learn">scikit-learn - Wikipedia</a></li>
<li><a href="https://doc.rust-lang.org/book/ch07-01-packages-and-crates.html">Packages and Crates - The Rust Programming Language</a></li>

</ul>
</details>

**标签**: `#AI-agents`, `#software-engineering`, `#Rust`, `#machine-learning`, `#developer-tools`

---

<a id="item-4"></a>
## [ChatGPT 周活跃用户近 10 亿，付费订阅用户突破 5000 万](https://9to5mac.com/2026/02/27/chatgpt-approaching-1-billion-weekly-active-users/) ⭐️ 8.0/10

OpenAI 披露，ChatGPT 的周活跃用户数已达 9 亿，较 18 个月前的 2 亿增长了 350%，正逼近 10 亿大关。同时，个人付费订阅用户数已突破 5000 万，占用户总数的 5%以上，且 2026 年 1 月和 2 月的新增订阅量创下历史新高。 这些数据表明 ChatGPT 实现了爆炸性增长并已进入主流市场，巩固了其作为主导性 AI 平台的地位。庞大的付费用户基数证明了其强大的商业可行性，也意味着用户越来越依赖其高级功能，这些功能正深度集成到苹果 iOS 和开发者工具等主要生态系统中。 这一增长部分得益于战略集成，包括在 iOS 18 中与 Siri 的深度集成，用户可通过 Siri 启用 ChatGPT 以获得更深入的答案。此外，苹果计划在未来的 iOS 更新中引入 Google Gemini，并与 Anthropic 合作在 Xcode 26.3 中提供 AI 编程支持，从而扩展了 ChatGPT 在苹果生态系统内的触达范围。

telegram · zaihuapd · Feb 28, 03:23

**背景**: ChatGPT 是由 OpenAI 开发的大型语言模型（LLM），能够生成类人文本、回答问题并协助完成各种任务。Apple Intelligence 是集成在苹果操作系统中的一套 AI 功能。Siri 是苹果内置的语音助手。Xcode 是苹果的集成开发环境（IDE），用于为苹果平台开发软件。Xcode 26.3 中引入的智能体编码（Agentic coding）指的是一种开发范式，即由 AI 智能体（如来自 Anthropic 和 OpenAI 的智能体）协助或自动化部分编码过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/guide/iphone/use-chatgpt-with-apple-intelligence-iph00fd3c8c2/ios">Use ChatGPT with Apple Intelligence on iPhone - Apple Support</a></li>
<li><a href="https://www.apple.com/newsroom/2026/02/xcode-26-point-3-unlocks-the-power-of-agentic-coding/">Xcode 26.3 unlocks the power of agentic coding - Apple</a></li>
<li><a href="https://vertu.com/ai-tools/apple-siri-google-gemini-integration-ai-revolution-coming-to-ios-in-2026/">Apple Siri Google Gemini Integration 2026 | Specs & Rollout</a></li>

</ul>
</details>

**标签**: `#AI`, `#ChatGPT`, `#User Metrics`, `#Platform Integration`, `#Industry Trends`

---

<a id="item-5"></a>
## [青龙面板遭.fullgc 挖矿木马植入，导致 CPU 占用率达 800%](https://t.me/zaihuapd/39934) ⭐️ 8.0/10

2026 年 2 月 7 日，多名用户发现流行的定时任务管理平台青龙面板被名为.fullgc 的挖矿木马植入，导致服务器 CPU 占用率异常飙升至 800%。该木马通过篡改 config.sh 配置文件实现持久化，并能根据系统架构自动下载恶意程序。 这是一起重大的安全事件，因为青龙面板被广泛用于服务器自动化，这意味着许多暴露在公网的管理服务器可能被劫持用于非法挖矿，导致严重的性能下降和运营成本增加。此次攻击凸显了暴露管理界面的风险，以及针对流行开源工具的加密货币挖矿恶意软件的持续威胁。 安全分析判定该程序属于 SusMiner 家族，主要通过连接 XMR（门罗币）矿池进行非法挖矿。暴露于公网 IPv4 环境的服务器是其主要攻击目标，建议用户检查/ql/data/db/路径下的隐藏文件。

telegram · zaihuapd · Feb 28, 13:16

**背景**: 青龙面板是一个开源的定时任务管理平台，支持 Python3、JavaScript、Shell 和 TypeScript，通常通过 Docker 部署，用于自动化运行脚本和任务。像此次的 SusMiner 变种这样的加密劫持恶意软件，会秘密劫持受害者的计算资源来挖掘门罗币（XMR）等加密货币，门罗币因其隐私特性而受此类攻击青睐。持久化机制允许恶意软件在系统重启后依然存活，通常通过修改系统文件或配置实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/whyour/qinglong">GitHub - whyour/qinglong: 支持 Python3、JavaScript、Shell ...</a></li>
<li><a href="https://www.pcrisk.com/removal-guides/12913-xmr-miner-virus">XMR Miner Virus - Easy removal steps (updated)</a></li>

</ul>
</details>

**标签**: `#security`, `#malware`, `#server-security`, `#cryptojacking`, `#open-source-security`

---

<a id="item-6"></a>
## [Google Chrome 默认自动下载 4GB 本地 AI 模型 Gemini Nano](https://winaero.com/google-chrome-secretly-downloads-huge-local-ai-models/) ⭐️ 7.0/10

Google Chrome 浏览器被发现在默认配置下会自动下载一个名为 'weights.bin'、大小约 4GB 的本地 AI 模型文件。该文件用于支持浏览器内置的 Prompt API、翻译及摘要等 AI 功能。 此举标志着谷歌将强大的设备端 AI 直接集成到浏览器中的重大举措，旨在为 AI 功能提供更快的响应速度和更好的隐私保护。然而，未经明确用户同意就自动下载大文件，引发了关于软件行为透明度、用户对磁盘空间使用的控制权以及此举所开创的先例的严重担忧。 该模型文件与 Gemini Nano 相关，这是谷歌 Gemini 大语言模型家族中为设备端运行设计的紧凑版本。用户可以通过禁用实验性标志并手动删除文件来释放磁盘空间，但这会导致相关的 AI 功能失效。

telegram · zaihuapd · Feb 28, 05:02

**背景**: Gemini 是谷歌 DeepMind 开发的多模态大语言模型（LLM）系列，是 LaMDA 和 PaLM 2 等模型的继任者。Chrome 的 Prompt API 是一个开发者接口，允许网络应用向这些本地 AI 模型发送自然语言请求，从而实现诸如聊天机器人和内容摘要等可以离线工作的功能。'weights.bin' 文件是存储神经网络模型学习到的参数（权重）的常见格式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(language_model)">Gemini (language model ) - Wikipedia</a></li>
<li><a href="https://developer.chrome.com/docs/ai/prompt-api">The Prompt API | AI on Chrome | Chrome for Developers</a></li>
<li><a href="https://medium.com/@ch.mittendorf/navigating-model-weight-file-formats-safetensors-bin-pt-hdf5-and-beyond-97266a621bdf">Navigating Model Weight File Formats: .safetensors, .bin, .pt, HDF5 ...</a></li>

</ul>
</details>

**标签**: `#Google Chrome`, `#Local AI`, `#Privacy`, `#Browser`, `#Gemini`

---

<a id="item-7"></a>
## [韩国国税厅误曝硬件钱包助记词，导致 480 万美元加密货币被转走](https://www.mk.co.kr/cn/stock/11974731) ⭐️ 7.0/10

韩国国税厅在公布对欠税人员的现场搜查成果时，将查封的一台 Ledger 硬件钱包的完整助记词公开在新闻资料中，导致该钱包内价值约 480 万美元的 400 万个 PRTG 代币被转走。大约 20 小时后，相关代币被全部退回原钱包。 这一事件凸显了政府机构在处理查封的数字资产时出现了根本性的安全失误，损害了公众对机构管理加密货币能力的信任。它暴露了在保护敏感加密信息程序上的系统性漏洞，对全球范围内的法律查封和资产安全都可能产生影响。 受影响的地址中，至少有 3 个自 2023 年 1 月后就不活跃，这些钱包合计持有 PRTG 总供应量的 40%。PRTG 代币流动性极低，仅在 MEXC 交易所上线，日成交额约 332 美元，这意味着仅卖出 59 美元就可能导致其价格下跌 2%。

telegram · zaihuapd · Feb 28, 11:27

**背景**: 助记词（或恢复短语）是由加密货币钱包生成的一系列单词，拥有它就意味着拥有对应钱包内资产的完全控制权。像 Ledger 这样的硬件钱包是物理设备，旨在将助记词离线保存以确保安全，因此助记词的数字曝光是一次灾难性的安全漏洞。加密货币自我托管的基本原则是绝不分享或数字化存储助记词。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ledger.com/academy/hardwarewallet/best-ways-to-protect-your-recovery-phrase">How to Keep Your Seed Phrase Secure - Ledger</a></li>
<li><a href="https://decrypt.co/359404/ethereum-tokens-swiped-returned-south-korean-tax-service">Ethereum Tokens Swiped, Returned After South Korean Tax ... - Decrypt</a></li>

</ul>
</details>

**标签**: `#cryptocurrency`, `#security`, `#government`, `#blockchain`, `#hardware-wallet`

---

<a id="item-8"></a>
## [摩托罗拉内部演示文稿泄露，暗示与 GrapheneOS 合作，首款非 Pixel 设备或于 2027 年面世](https://grapheneos.social/@GrapheneOS/116115497756691311) ⭐️ 7.0/10

一张最初发布在 Reddit 上的摩托罗拉内部演示文稿截图泄露，其中明确将 GrapheneOS 列在该公司的安全功能板块内，强烈暗示双方已达成合作。GrapheneOS 项目随后在 Mastodon 上确认，官方 OEM 合作伙伴公告定于 2026 年 3 月发布，相关设备计划于 2027 年推出。 这标志着 GrapheneOS 可能首次突破其对 Google Pixel 设备的独家支持，极大地扩展了其可及性和市场影响力。与摩托罗拉（隶属于联想集团，并专注于企业安全业务）这样的大型 OEM 厂商合作，将为这款注重隐私的操作系统带来巨大的可信度，并加速其在商业市场和安全意识强的消费者市场中的采用。 泄露的截图很快被 r/GrapheneOS 版块的版主删除，但已广泛传播。截至发稿，GrapheneOS 和摩托罗拉双方均未就泄露内容发表官方声明，相关信息尚未得到相关公司的正式确认。

telegram · zaihuapd · Feb 28, 12:38

**背景**: GrapheneOS 是一个基于 Android 开源项目（AOSP）、专注于隐私和安全的移动操作系统，以其强化的安全功能和默认的隐私保护而闻名。由于 Google Pixel 设备强大的硬件安全能力，GrapheneOS 历史上仅官方支持部分 Pixel 机型。隶属于联想集团的摩托罗拉解决方案公司为企业客户提供企业移动性管理和安全解决方案（如“moto-safe”），在安全移动设备市场中占有一席之地。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.allthingssecured.com/identity-protection/android-vs-grapheneos-compared/">Android vs GrapheneOS: Privacy, Security & Features Compared</a></li>
<li><a href="https://www.reddit.com/r/GrapheneOS/comments/1r7m2q9/grapheneos_project_member_confirms_oem_partner/">GrapheneOS project member confirms OEM Partner unveil in March 2026</a></li>
<li><a href="https://www.motorola.com/business/moto-safe">moto-safe - Motorola</a></li>

</ul>
</details>

**标签**: `#mobile-security`, `#privacy`, `#operating-systems`, `#hardware`, `#android`

---