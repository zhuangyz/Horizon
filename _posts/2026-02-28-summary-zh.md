---
layout: default
title: "Horizon Summary: 2026-02-28 (ZH)"
date: 2026-02-28
lang: zh
---

> From 24 items, 8 important content pieces were selected

---

1. [AI 公司抵制政府将 AI 模型用于监控和自主武器的要求](#item-1) ⭐️ 8.0/10
2. [AI 编码怀疑论者详细记录实验，包括将 scikit-learn 移植到 Rust](#item-2) ⭐️ 8.0/10
3. [ChatGPT 周活跃用户达 9 亿，付费订阅用户突破 5000 万](#item-3) ⭐️ 8.0/10
4. [青龙面板遭.fullgc 挖矿木马植入，导致 CPU 占用率达 800%](#item-4) ⭐️ 8.0/10
5. [安全专家呼吁开发者停止使用通行密钥加密用户数据](#item-5) ⭐️ 7.0/10
6. [Google Chrome 默认自动下载 4GB 本地 AI 模型 Gemini Nano](#item-6) ⭐️ 7.0/10
7. [韩国国税厅误曝硬件钱包助记词，导致 480 万美元加密货币被转走](#item-7) ⭐️ 7.0/10
8. [摩托罗拉与 GrapheneOS 合作遭泄露，首款非 Pixel 设备或于 2027 年面世](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [AI 公司抵制政府将 AI 模型用于监控和自主武器的要求](https://notdivided.org/) ⭐️ 8.0/10

一项公开呼吁要求 AI 公司拒绝政府提出的、将其 AI 模型用于国内大规模监控和无需人类监督的自主杀伤系统的要求。以 Anthropic 为代表的公司明确表示，其模型不能用于这些目的。 这标志着 AI 领域企业责任的一个关键时刻，为科技公司如何在伦理红线与政府压力之间抉择树立了先例。其结果可能影响全球关于 AI 军事化、以及数字时代国家安全与公民自由之间平衡的规范。 据报道，具体要求来自美国战争部，旨在取消对将 AI 用于国内大规模监控和全自主武器的限制。尽管 Anthropic 等公司支持将 AI 用于合法的外国情报工作，但他们坚决反对对本国公民进行监控。

hackernews · BloondAndDoom · Feb 28, 00:54

**背景**: 致命性自主武器系统（LAWS），常被称为“屠宰机器人”或“杀手机器人”，是指利用 AI 在没有人类干预的情况下识别、选择和攻击目标的武器。利用 AI 进行国内大规模监控涉及对人群活动、通信和行踪的海量数据进行分析。伦理辩论的核心在于将人类判断从生死决策中移除，以及国家监控可能达到的前所未有的规模和侵入性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lethal_autonomous_weapon">Lethal autonomous weapon - Wikipedia</a></li>
<li><a href="https://officechai.com/ai/anthropic-defies-us-govt-says-its-models-cant-be-used-for-domestic-surveillance-or-autonomous-weapons/">Anthropic Defies US Govt, Says Its Models Can't Be Used For Domestic ...</a></li>
<li><a href="https://www.commoncause.org/resources/pete-hegseth-vs-anthropic-read-our-letter-on-ai-surveillance/">Pete Hegseth vs. Anthropic: Read Our Letter On AI Surveillance</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示出对政府越权行为更广泛影响的深切担忧，用户担心此先例可能被用来惩罚任何令政府不满的公司。另一些人则从国际视角指出国内监控政策的虚伪性，还有一些人警告说，如果武器化的 AI 系统被黑客攻击或滥用，所要求的能力最终可能对当权者造成反噬。

**标签**: `#AI Ethics`, `#Government Surveillance`, `#National Security`, `#Corporate Responsibility`, `#Autonomous Weapons`

---

<a id="item-2"></a>
## [AI 编码怀疑论者详细记录实验，包括将 scikit-learn 移植到 Rust](https://simonwillison.net/2026/Feb/27/ai-agent-coding-in-excessive-detail/#atom-everything) ⭐️ 8.0/10

此前持怀疑态度的开发者 Max Woolf 详细记录了一系列使用 AI 编码代理完成的、复杂度递增的项目，最终尝试将核心机器学习库 scikit-learn 从 Python 移植到 Rust。他发现，像 Anthropic 的 Opus 4.6 和 OpenAI 的 Codex 5.3 这样的模型，能够完成那些原本需要他手动花费数月时间的复杂任务。 这份来自怀疑论者的详细实践记录，为 AI 辅助编码能力的显著飞跃提供了强有力的实践证据，表明这些工具现在已能处理实质性的、真实的软件工程项目。这预示着开发者工作流程可能发生转变，AI 代理可以加速甚至自主处理诸如库移植和算法实现等复杂任务。 这个雄心勃勃的 'rustlearn' 项目不仅旨在用 Rust 复现 scikit-learn 的逻辑回归和 k-means 聚类等算法，还力求在速度上超越原始的 Python 实现。作者特别强调了 2025 年 11 月左右发布的模型性能有巨大飞跃，指出其性能比几个月前的模型'好了一个数量级'。

rss · Simon Willison · Feb 27, 20:43

**背景**: AI 编码代理是使用大语言模型来理解自然语言指令并生成、调试或重构代码的自主或半自主软件工具。Scikit-learn 是一个基础的、开源的 Python 机器学习库，被广泛认为是经典机器学习算法的行业标准。Rust 是一种以其性能和内存安全性著称的系统编程语言，而 'crate' 是 Rust 中对代码包或库的称呼。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cssauthor.com/best-ai-coding-agents/">Best AI Coding Agents 2026: The Senior Editor’s Guide</a></li>
<li><a href="https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html">LinearRegression — scikit - learn 1.8.0 documentation</a></li>
<li><a href="https://doc.rust-lang.org/book/ch07-01-packages-and-crates.html">Packages and Crates - The Rust Programming Language</a></li>

</ul>
</details>

**标签**: `#AI-agents`, `#software-development`, `#Rust`, `#machine-learning`, `#automation`

---

<a id="item-3"></a>
## [ChatGPT 周活跃用户达 9 亿，付费订阅用户突破 5000 万](https://9to5mac.com/2026/02/27/chatgpt-approaching-1-billion-weekly-active-users/) ⭐️ 8.0/10

OpenAI 披露，ChatGPT 的周活跃用户数已达 9 亿，较 18 个月前的 2 亿增长了 350%，正逼近 10 亿大关。同时，个人付费订阅用户数突破 5000 万，占比超过 5%，且 2026 年 1 月和 2 月的新增订阅量创下历史新高。 这些数据表明 ChatGPT 的用户采纳规模巨大且增长迅速，巩固了其作为主流消费级 AI 平台的地位。与苹果生态（如 iOS 18 中的 Siri）的深度集成，以及未来可能与 Google Gemini 和 Anthropic 在开发者工具上的合作，都预示着其影响力正扩展到整个科技行业。 报告强调了其战略集成，包括 ChatGPT 通过 iOS 18 与 Siri 的深度集成。此外，苹果计划在未来的 iOS 26.5 更新中引入 Google Gemini，并正与 Anthropic 合作，在苹果的集成开发环境 Xcode 内提供 AI 编程支持。

telegram · zaihuapd · Feb 28, 03:23

**背景**: ChatGPT 是由 OpenAI 开发的对话式 AI 聊天机器人。Anthropic 是一家 AI 安全与研究公司，以其 Claude 系列大语言模型而闻名。Xcode 是苹果公司的集成开发环境（IDE），用于为 macOS、iOS、iPadOS 等苹果平台开发软件。Xcode 的最新版本（如 26.3 版）已开始集成 AI 编程助手来帮助开发者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://developer.apple.com/documentation/xcode/writing-code-with-intelligence-in-xcode">Writing code with intelligence in Xcode - Apple Developer</a></li>
<li><a href="https://appleinsider.com/articles/26/02/26/xcode-with-vibecoding-ai-agents-to-help-build-apps-is-now-available">Xcode now runs with AI agents to analyze, modify & build apps</a></li>

</ul>
</details>

**标签**: `#AI`, `#ChatGPT`, `#User Metrics`, `#Apple Integration`, `#Industry Trends`

---

<a id="item-4"></a>
## [青龙面板遭.fullgc 挖矿木马植入，导致 CPU 占用率达 800%](https://t.me/zaihuapd/39934) ⭐️ 8.0/10

2026 年 2 月 7 日，多名用户发现流行的定时任务管理面板青龙面板被名为.fullgc 的挖矿木马感染，导致服务器 CPU 占用率异常飙升至 800%。该木马通过篡改`config.sh`配置文件实现持久化驻留，并能根据系统架构自动下载对应的恶意程序。 此次事件暴露了广泛使用的、暴露在公网的服务管理工具所面临的重大安全风险，它们可能成为劫持计算资源进行非法挖矿的攻击载体。这凸显了开源基础设施面临的持续性威胁，以及对受影响服务器运营者可能造成的重大财务和运营损失。 安全分析判定该木马属于 SusMiner 家族，主要通过连接 XMR（门罗币）矿池进行非法加密货币挖矿。主要攻击目标是暴露在公网 IPv4 环境下的服务器，建议用户检查`/ql/data/db/`路径下的隐藏文件。

telegram · zaihuapd · Feb 28, 13:16

**背景**: 青龙面板是一个基于 Docker 的开源定时任务管理面板，支持 TypeScript、JavaScript、Python 和 Shell 脚本，常用于自动化执行各类网络任务。挖矿木马（如.fullgc 变种）会秘密劫持计算机的处理能力来为攻击者挖掘加密货币以牟利，通常导致设备性能严重下降。SusMiner 家族是专门从事此类非法挖矿活动的已知恶意软件家族。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hub.docker.com/r/whyour/qinglong">whyour/qinglong - Docker Image</a></li>
<li><a href="https://cybersecuritynews.com/advanced-crypto-mining-malware/">Advanced Crypto Mining Malware Spreads Through External ...</a></li>
<li><a href="https://hunt.io/malware-families">The Most Popular Malware Families - hunt.io</a></li>

</ul>
</details>

**标签**: `#security`, `#malware`, `#cryptojacking`, `#server-security`, `#incident-response`

---

<a id="item-5"></a>
## [安全专家呼吁开发者停止使用通行密钥加密用户数据](https://simonwillison.net/2026/Feb/27/passkeys/#atom-everything) ⭐️ 7.0/10

身份认证行业专家 Tim Cappalli 直接呼吁开发者停止使用通行密钥（passkeys）来加密用户数据，并警告称，当用户不可避免地丢失其通行密钥时，这种做法将导致数据永久丢失。这一警告特别针对 WebAuthn PRF（伪随机函数）扩展的滥用，一些服务利用该扩展从通行密钥生成加密密钥。 这一点很重要，因为它凸显了安全目标与用户体验之间的关键冲突：使用通行密钥进行加密会创建一个不可逆的单点故障。如果这种模式继续不受控制，通行密钥的广泛采用反而可能导致普通用户在无法访问其认证器时，遭受大规模、不可恢复的数据丢失。 核心问题在于，WebAuthn API 和通行密钥的设计初衷主要是用于身份验证，而非通用加密。虽然 PRF 扩展可以确定性地生成密钥，但它缺乏密钥恢复或托管机制，这意味着一旦通行密钥丢失，用此类密钥加密的任何数据都将永久无法访问。

rss · Simon Willison · Feb 27, 22:49

**背景**: 通行密钥是基于 WebAuthn 构建的无密码身份验证标准，它使用公钥密码学，其中私钥保留在用户设备（如手机或安全密钥）上，公钥则由服务存储。它们因能抵抗网络钓鱼且比密码更易于使用而受到赞誉。WebAuthn PRF 扩展是一项功能，允许通行密钥的认证器根据提供的“盐值”生成对称加密密钥，从而为端到端加密等用途实现确定性的密钥派生。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.corbado.com/blog/passkeys-prf-webauthn">Passkeys & WebAuthn PRF for End-to-End Encryption (2026)</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAuthn">WebAuthn - Wikipedia</a></li>
<li><a href="https://stackoverflow.com/questions/59837620/webauthn-for-encryption">Webauthn for encryption - Stack Overflow</a></li>

</ul>
</details>

**标签**: `#security`, `#passkeys`, `#usability`, `#encryption`, `#authentication`

---

<a id="item-6"></a>
## [Google Chrome 默认自动下载 4GB 本地 AI 模型 Gemini Nano](https://winaero.com/google-chrome-secretly-downloads-huge-local-ai-models/) ⭐️ 7.0/10

Google Chrome 浏览器被发现在默认配置下自动下载一个名为 'weights.bin'、大小约 4GB 的本地 AI 模型文件。该文件包含 Gemini Nano 模型，主要用于支持 Prompt API、翻译及摘要等内置 AI 功能。 这一做法代表了主流浏览器部署 AI 方式的重大转变，直接影响用户存储空间，并引发了关于透明度和用户同意的疑问。它凸显了行业为追求速度和隐私而推动设备端 AI 的趋势，但其代价是自动、大规模的资源消耗。 用户可以通过在 Chrome 中禁用相关实验性标志并手动删除对应文件夹来释放磁盘空间，但这会导致相关 AI 功能失效。该模型设计为本地运行，旨在通过不将数据发送到外部服务器来提高响应速度并保护用户隐私。

telegram · zaihuapd · Feb 28, 05:02

**背景**: Gemini 是由 Google DeepMind 开发的多模态大语言模型（LLM）系列。'weights.bin' 文件是存储模型学习参数（对其功能至关重要）的常见格式。Chrome 内置的 Prompt API（从版本 138 开始提供）允许开发者访问这个本地 Gemini Nano 模型，为扩展程序构建设备端 AI 功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(language_model)">Gemini (language model) - Wikipedia</a></li>
<li><a href="https://medium.com/@dobidev/building-a-privacy-first-summarizer-with-chrome-prompt-api-and-structured-output-25d51759de9b">Building a Privacy-First Summarizer with Chrome Prompt API and...</a></li>
<li><a href="https://medium.com/@ch.mittendorf/navigating-model-weight-file-formats-safetensors-bin-pt-hdf5-and-beyond-97266a621bdf">Navigating Model Weight File Formats: .safetensors, .bin, .pt ...</a></li>

</ul>
</details>

**标签**: `#Google Chrome`, `#AI Models`, `#Privacy`, `#Browser`, `#Local AI`

---

<a id="item-7"></a>
## [韩国国税厅误曝硬件钱包助记词，导致 480 万美元加密货币被转走](https://www.mk.co.kr/cn/stock/11974731) ⭐️ 7.0/10

韩国国税厅近日在公布对欠税人员的现场搜查成果时，将查封的一台 Ledger 硬件钱包的完整助记词未加遮挡地公开在新闻资料中。这导致该钱包内价值约 480 万美元的 400 万个 PRTG 代币被转走，但约 20 小时后，代币被全部退回原地址。 这一事件突显了一个主要政府机构在加密货币安全管理上的重大制度性失误，表明基本的安全疏漏可能导致即时的高价值损失。它揭示了在法律程序中，被查封的加密资产所面临的脆弱性，并对当局管理数字资产的能力提出了严重质疑。 被曝光的助记词来自一台 Ledger 硬件钱包，图像未经过任何遮挡处理。受影响的至少 3 个钱包自 2023 年 1 月后便不活跃，它们合计掌握了 PRTG 代币总供应量的 40%。PRTG 代币流动性极低，仅在 MEXC 交易所上线，日成交额约 332 美元，卖出 59 美元就可能导致价格下跌 2%。

telegram · zaihuapd · Feb 28, 11:27

**背景**: 助记词（也称为秘密恢复短语或备份短语）是一个由 12、18 或 24 个单词组成的列表，它存储了恢复和访问加密货币钱包内资金所需的全部信息。像 Ledger 这样的硬件钱包会离线生成和存储这些助记词以提供增强的安全性，因为私钥永远不会离开设备。任何拥有钱包助记词的人都能完全控制该钱包中存储的所有资产。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ledger.com/academy/basic-basics/2-how-to-own-crypto/whats-a-secret-recovery-phrase">What is a Seed Phrase (Secret Recovery Phrase)? | Ledger</a></li>
<li><a href="https://www.thecryptomerchant.com/blogs/resources/hardware-wallet-recovery-seeds-explained">Hardware Wallet Recovery Seeds Explained – The Crypto Merchant</a></li>
<li><a href="https://en.bitcoin.it/wiki/Seed_phrase">Seed phrase - Bitcoin Wiki</a></li>

</ul>
</details>

**标签**: `#cryptocurrency`, `#security`, `#blockchain`, `#institutional-failure`, `#South-Korea`

---

<a id="item-8"></a>
## [摩托罗拉与 GrapheneOS 合作遭泄露，首款非 Pixel 设备或于 2027 年面世](https://grapheneos.social/@GrapheneOS/116115497756691311) ⭐️ 7.0/10

一张泄露的摩托罗拉内部演示文稿截图显示，GrapheneOS 被明确列入该公司的安全功能板块，这强烈暗示双方已达成合作。随后，GrapheneOS 官方 Mastodon 账号透露，OEM 合作伙伴的公告定于 2026 年 3 月发布，相关设备计划于 2027 年推出。 这标志着 GrapheneOS 可能首次将其支持范围扩展到谷歌 Pixel 设备之外，有望显著提升其在移动安全市场的采用率和公信力。与摩托罗拉这样隶属于联想集团、专注于企业安全的大型 OEM 合作，可能将注重隐私、去谷歌化的移动设备带给更广泛的用户群体。 泄露的截图最初发布在 Reddit 的 r/GrapheneOS 版块，随后被版主删除，但已广泛传播。截至报道时，GrapheneOS 和摩托罗拉双方均未就合作细节发布官方声明予以确认。

telegram · zaihuapd · Feb 28, 12:38

**背景**: GrapheneOS 是一个基于 Android 开源项目（AOSP）、专注于隐私和安全的移动操作系统。它以其强大的安全增强功能而闻名，包括完整且及时的安全补丁，并且历史上仅官方支持谷歌 Pixel 设备，因为后者具备强大的硬件安全特性。摩托罗拉解决方案（Motorola Solutions）是一家提供安全与安防产品及服务的技术公司，其产品包括用于移动数据安全和终端管理的 ThinkShield 平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grapheneos.org/features">Features overview - GrapheneOS</a></li>
<li><a href="https://tbot.substack.com/p/grapheneos-new-oem-partnership">GrapheneOS Confirms New OEM Partnership for Next-Gen Secure ...</a></li>
<li><a href="https://www.motorola.com/business/thinkshield/p">Motorola ThinkShield for Mobile Data Security | Motorola ...</a></li>

</ul>
</details>

**标签**: `#mobile-security`, `#privacy`, `#android`, `#grapheneos`, `#oem-partnership`

---