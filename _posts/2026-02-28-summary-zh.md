---
layout: default
title: "Horizon Summary: 2026-02-28 (ZH)"
date: 2026-02-28
lang: zh
---

> From 24 items, 8 important content pieces were selected

---

1. [AI 公司面临政府监控与军事合作的伦理十字路口](#item-1) ⭐️ 8.0/10
2. [安全专家呼吁开发者停止使用 Passkey 加密用户数据](#item-2) ⭐️ 8.0/10
3. [怀疑论者通过尝试将 scikit-learn 移植到 Rust 来测试 AI 编程智能体](#item-3) ⭐️ 8.0/10
4. [ChatGPT 周活跃用户达 9 亿，付费订阅用户突破 5000 万](#item-4) ⭐️ 8.0/10
5. [Google Chrome 默认下载 4GB 本地 AI 模型 Gemini Nano](#item-5) ⭐️ 7.0/10
6. [韩国国税厅误曝硬件钱包助记词，导致 480 万美元加密货币被转走](#item-6) ⭐️ 7.0/10
7. [摩托罗拉内部演示文稿泄露，揭示与 GrapheneOS 合作，首款非 Pixel 设备或于 2027 年面世](#item-7) ⭐️ 7.0/10
8. [青龙面板遭.fullgc 挖矿木马植入，导致 CPU 占用率飙升至 800%](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [AI 公司面临政府监控与军事合作的伦理十字路口](https://notdivided.org/) ⭐️ 8.0/10

一场围绕 notdivided.org 网站的公开讨论已经出现，凸显了人们对 AI 公司与政府监控项目合作以及涉足军事技术领域日益增长的担忧。讨论特别提到了 OpenAI 据称与五角大楼达成的协议，并对围绕此类合作的伦理框架提出了质疑。 此事至关重要，因为将先进 AI 整合到监控和军事系统中，引发了关于隐私、公民自由以及技术武器化的深刻问题。领先 AI 公司当前做出的决定，将为企业的社会责任、政府权力越界以及管理军民两用 AI 技术的全球规范树立先例。 讨论指向了 OpenAI 与美国国防部之间一项被报道的具体协议，据称该协议包含了伦理保障措施。批评者认为，尽管有美国国防部等实体声明的伦理原则，此类合作仍可能使大规模监控能力常态化，并扩大 AI 在战争中的应用。

hackernews · BloondAndDoom · Feb 28, 00:54

**背景**: 人工智能（AI）指的是能够执行通常需要人类智能的任务的计算机系统。政府监控项目利用技术监控人群，通常出于安全目的。近年来，人脸识别和预测分析等 AI 能力极大地增强了此类监控的规模和效率。当它们的产品被寻求用于军事或情报应用时，许多科技公司都面临着伦理困境，需要在创新、利润和社会责任之间取得平衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.politico.com/news/2026/02/28/openai-announces-new-deal-with-pentagon-including-ethical-safeguards-00805546">OpenAI announces new deal with Pentagon — including ethical safeguards</a></li>
<li><a href="https://www.brookings.edu/articles/how-ai-can-enable-public-surveillance/">How AI can enable public surveillance</a></li>
<li><a href="https://www.war.gov/News/Releases/Release/Article/2091996/dod-adopts-ethical-principles-for-artificial-intelligence/">DOD Adopts Ethical Principles for Artificial Intelligence</a></li>

</ul>
</details>

**社区讨论**: 社区情绪以批评和担忧为主，强调了其中的虚伪性和潜在危险。主要观点包括：批评 OpenAI 尽管公开表明伦理立场，却与“战争部”关系密切；担心为美国开发的监控能力可能被其他国家用来对付美国公民；以及担忧政府采购规则可能被武器化，用于因政治原因惩罚公司。部分评论提出了一种报复性逻辑，警告那些要求监控 AI 的人自己也可能成为目标。

**标签**: `#AI Ethics`, `#Government Surveillance`, `#Military Technology`, `#Corporate Responsibility`, `#National Security`

---

<a id="item-2"></a>
## [安全专家呼吁开发者停止使用 Passkey 加密用户数据](https://simonwillison.net/2026/Feb/27/passkeys/#atom-everything) ⭐️ 8.0/10

安全专家 Tim Cappalli 向身份识别行业发出公开呼吁，敦促开发者停止使用 Passkey 来加密用户数据。他警告称，这种做法存在永久性数据丢失的风险，因为用户经常丢失他们的 Passkey，并且可能没有意识到他们的数据已被不可逆地加密。 这一警告凸显了对一项核心认证技术的严重误用，可能导致最终用户大规模、不可逆的数据丢失。它之所以重要，是因为它抵制了使用 WebAuthn PRF 扩展进行客户端加密的日益增长的趋势，并强调 Passkey 应专注于其作为防钓鱼认证凭证的主要安全角色。 该警告特别针对 WebAuthn 伪随机函数（PRF）扩展的使用，该扩展允许 Passkey 生成确定性的加密密钥。一个关键的注意事项是，WebAuthn API 的设计旨在防止直接访问或操作私钥，这意味着如果 Passkey（持有私钥的认证器）丢失，密钥恢复将是不可能的。

rss · Simon Willison · Feb 27, 22:49

**背景**: Passkey 是一种基于 WebAuthn 标准的无密码认证技术，它使用公钥密码学，其中公钥由服务存储，私钥则安全地存储在用户的设备上（如手机或安全密钥）。WebAuthn PRF 扩展是一项功能，允许这些 Passkey 生成一致的加密密钥，一些开发者已开始将其用于客户端数据加密。与存储和管理秘密的传统密码管理器不同，Passkey 主要设计用于在登录过程中证明身份。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bitwarden.com/blog/prf-webauthn-and-its-role-in-passkeys/">PRF WebAuthn and its role in passkeys | Bitwarden</a></li>
<li><a href="https://www.corbado.com/blog/passkeys-prf-webauthn">Passkeys & WebAuthn PRF for End-to-End Encryption (2026)</a></li>
<li><a href="https://github.com/w3c/webauthn/issues/1595">Can the private keys be used for other cryptographic operations? · Issue #1595 · w3c/webauthn</a></li>

</ul>
</details>

**标签**: `#security`, `#authentication`, `#passkeys`, `#cryptography`, `#usability`

---

<a id="item-3"></a>
## [怀疑论者通过尝试将 scikit-learn 移植到 Rust 来测试 AI 编程智能体](https://simonwillison.net/2026/Feb/27/ai-agent-coding-in-excessive-detail/#atom-everything) ⭐️ 8.0/10

2026 年 2 月，AI 研究员兼怀疑论者 Max Woolf 发表了一份详细报告，记录了他在一系列难度递增的项目上测试 AI 编程智能体的过程，最终尝试将核心机器学习库 scikit-learn 从 Python 移植到 Rust，并创建了一个名为 `rustlearn` 的 crate。他发现，像 Opus 4.6/Codex 5.3 这样的模型比几个月前发布的模型性能提升了一个数量级，成功完成了他预期需要数月才能完成的复杂任务。 这项真实世界的高难度测试展示了 AI 编程智能体在实际能力上的重大飞跃，超越了简单的代码生成，有可能协助完成像库移植这样大规模、复杂的软件工程项目。这标志着一个转变，即 AI 智能体可能成为加速机器学习等性能关键领域开发的有效工具，而 Rust 的速度和安全性在这些领域具有优势。 该项目 `rustlearn` 的目标不仅是在 Rust 中复现 scikit-learn 的算法（如逻辑回归和 k-means 聚类），还要实现更快的版本，以期超越原始的 Python 实现。作者的经历突出了一个关键痛点：像 Opus 4.6 这样的模型改进幅度之大令人难以置信，以至于在描述时很难不让人觉得是在夸大其词。

rss · Simon Willison · Feb 27, 20:43

**背景**: AI 编程智能体是基于大型语言模型（LLM）构建的 AI 系统，能够根据自然语言指令自主或半自主地编写、重构、调试和执行代码。2026 年的生态包括像 Claude Code、Cursor 和 Aider 这样能在代码库级别操作的工具。Scikit-learn 是一个基础且广泛使用的 Python 机器学习库。Rust 是一种系统编程语言，以其性能和内存安全性著称，因此成为移植性能敏感的 Python 代码的理想目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.qodo.ai/blog/best-ai-coding-assistant-tools/">Top 15 AI Coding Assistant Tools to Try in 2026</a></li>
<li><a href="https://github.com/Menonlab-Rich/rsklearn">GitHub - Menonlab-Rich/rsklearn: A collection of sklearn algorithms ...</a></li>
<li><a href="https://lib.rs/crates/rustlearn">rustlearn — system library interface for Rust // Lib.rs</a></li>

</ul>
</details>

**标签**: `#AI-agents`, `#software-development`, `#Rust`, `#machine-learning`, `#code-generation`

---

<a id="item-4"></a>
## [ChatGPT 周活跃用户达 9 亿，付费订阅用户突破 5000 万](https://9to5mac.com/2026/02/27/chatgpt-approaching-1-billion-weekly-active-users/) ⭐️ 8.0/10

OpenAI 披露，ChatGPT 的周活跃用户数已达 9 亿，较 18 个月前的 2 亿增长了 350%，正逼近 10 亿大关。同时，个人付费订阅用户数突破 5000 万，占比超过 5%，且 2026 年 1 月和 2 月的新增订阅量创下历史新高。 这一爆炸性增长表明 ChatGPT 已获得大规模主流采用，并巩固了其作为领先消费级 AI 平台的地位。庞大的付费用户群，加上与苹果 iOS 和 Siri 等主要生态系统的深度集成，标志着它已成功从一个免费的新奇工具，转型为一个可持续、深度嵌入且具有巨大收入潜力的服务。 此次集成不仅限于 ChatGPT，苹果还计划在 iOS 26.5 中引入 Google 的 Gemini，并与 Anthropic 合作在 Xcode 中提供 AI 编程支持。这些合作凸显了苹果的战略举措，即构建一个多模型 AI 助手生态系统，而非依赖单一供应商。

telegram · zaihuapd · Feb 28, 03:23

**背景**: ChatGPT 是由 OpenAI 开发的对话式 AI 聊天机器人，以其生成类人文本的能力而闻名。Anthropic 是一家 AI 安全研究公司，开发了 Claude 系列大语言模型。Xcode 是苹果公司的集成开发环境（IDE），用于为 macOS、iOS 和其他苹果平台构建软件。'Agentic coding'（智能体编码）指的是 AI 工具能够自主地与开发环境交互，以规划、编写和维护代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://www.apple.com/newsroom/2026/02/xcode-26-point-3-unlocks-the-power-of-agentic-coding/">Xcode 26.3 unlocks the power of agentic coding - Apple</a></li>
<li><a href="https://en.wikipedia.org/wiki/IOS_26">iOS 26 - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI`, `#ChatGPT`, `#User Metrics`, `#Tech Partnerships`, `#Apple Integration`

---

<a id="item-5"></a>
## [Google Chrome 默认下载 4GB 本地 AI 模型 Gemini Nano](https://winaero.com/google-chrome-secretly-downloads-huge-local-ai-models/) ⭐️ 7.0/10

Google Chrome 浏览器被发现在默认配置下自动下载一个约 4GB、名为 'weights.bin' 的本地 AI 模型文件。该文件主要用于支持 Prompt API、翻译及摘要等内置 AI 功能。 这标志着主流浏览器在 AI 部署方式上的重大转变，即默认进行大规模、本地的模型集成。它影响了用户的存储空间和隐私预期，并为浏览器为实现新功能而静默、自动下载大型 AI 资产开创了先例。 该模型是 Gemini Nano，这是谷歌为注重隐私和低延迟场景设计的本地基础模型。用户可以通过实验性标志禁用该功能并删除文件以释放空间，但这会导致相关的 AI 功能失效。

telegram · zaihuapd · Feb 28, 05:02

**背景**: Gemini Nano 是谷歌 Gemini AI 模型家族的轻量级版本，经过优化可直接在用户设备上运行，无需云端连接。Prompt API 是一个实验性的 Web API，允许网站和扩展程序使用 JavaScript 访问这些由浏览器提供的本地语言模型。浏览器中的本地 AI 旨在通过本地处理数据而非发送到远程服务器，来提供更快的响应和更强的隐私保护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.android.com/ai/gemini-nano">Gemini Nano | AI | Android Developers</a></li>
<li><a href="https://developer.chrome.com/docs/ai/prompt-api">The Prompt API | AI on Chrome | Chrome for Developers</a></li>
<li><a href="https://www.sitepoint.com/on-device-ai-for-the-web/">Web AI: Everything You Need to Know About On-Device AI for the Web</a></li>

</ul>
</details>

**标签**: `#Google Chrome`, `#Gemini Nano`, `#On-Device AI`, `#Browser Privacy`, `#AI Deployment`

---

<a id="item-6"></a>
## [韩国国税厅误曝硬件钱包助记词，导致 480 万美元加密货币被转走](https://www.mk.co.kr/cn/stock/11974731) ⭐️ 7.0/10

韩国国税厅在公布对欠税人员的现场搜查成果时，将查封的一台 Ledger 硬件钱包的完整助记词未加遮挡地公开在新闻资料中，导致相关钱包内价值约 480 万美元的 400 万个 PRTG 代币被转走。大约 20 小时后，这些代币被全部退回了原钱包。 这一事件凸显了政府机构在加密货币安全管理上的重大失误，展示了不当处理助记词可能带来的严重后果。它强调了即使对于机构行为者，数字资产也需要严格的安全协议，并对处理加密货币查封的当局的专业能力提出了质疑。 被泄露的助记词来自一台 Ledger 硬件钱包，且图像未经过任何遮挡处理。链上记录显示，至少 3 个自 2023 年 1 月后不活跃的钱包受影响，这些钱包合计掌握 PRTG 总供应量的 40%。PRTG 代币流动性极低，仅在 MEXC 交易所上线，日成交额约 332 美元，卖出 59 美元就可能让价格下跌 2%。

telegram · zaihuapd · Feb 28, 11:27

**背景**: 助记词（或恢复短语）是一系列单词，作为加密货币钱包的主密钥，任何人拥有它即可完全控制其中的资产。像 Ledger 这样的硬件钱包是物理设备，旨在将助记词离线存储以增强安全性。PRTG 代币（Pre-Retogeum）是 Ethereum 生态系统上的一种加密货币，市场规模和交易量都非常小。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://crypto-corner.com/2026/02/23/🛡️-importing-seed-phrase-into-a-hardware-wallet-dos-and-donts/">Importing Seed Phrase Into a Hardware Wallet: Do’s and Don’ts</a></li>
<li><a href="https://www.coingecko.com/en/coins/pre-retogeum">Pre-Retogeum Price: PRTG Live Price Chart, Market Cap & News Today | CoinGecko</a></li>
<li><a href="https://coinmarketcap.com/exchanges/mexc/">MEXC trade volume and market listings | CoinMarketCap</a></li>

</ul>
</details>

**标签**: `#cryptocurrency`, `#security`, `#government`, `#blockchain`, `#incident`

---

<a id="item-7"></a>
## [摩托罗拉内部演示文稿泄露，揭示与 GrapheneOS 合作，首款非 Pixel 设备或于 2027 年面世](https://grapheneos.social/@GrapheneOS/116115497756691311) ⭐️ 7.0/10

一张最初发布在 Reddit 的 r/GrapheneOS 版块的摩托罗拉内部演示文稿截图，在其安全功能板块中明确列出了 GrapheneOS，强烈暗示双方已达成正式合作协议。GrapheneOS 官方 Mastodon 账号于 2 月 22 日透露，关于 OEM 合作伙伴的公告定于 2026 年 3 月发布，相关设备计划于 2027 年推出。 这标志着 GrapheneOS 超越了其长期以来对 Google Pixel 设备的独占性，迈出了关键性的扩张一步，有望通过一家主要的智能手机制造商，将其强化的隐私和安全功能带给更广泛的用户。一次成功的合作可能显著提升以隐私为中心的移动操作系统的采用率，为安全移动生态系统引入更多竞争，并挑战标准 Android 在企业市场和安全意识强的消费者市场中的主导地位。 泄露的幻灯片虽被版主迅速删除，但已广泛传播，且 GrapheneOS 和摩托罗拉（隶属于联想集团）均未就合作细节发布官方声明予以确认。摩托罗拉近年来持续加强其企业移动安全产品线，拥有 Android Enterprise Recommended (AER)等认证，并主打其 ThinkShield 安全平台，这与潜在集成 GrapheneOS 的目标相吻合。

telegram · zaihuapd · Feb 28, 12:38

**背景**: GrapheneOS 是一个基于 Android 的非营利性开源移动操作系统，以其对安全和隐私的极致关注而闻名。由于其强大的硬件安全功能和及时的固件更新，该系统的开发和支持历史上几乎完全局限于 Google Pixel 设备。摩托罗拉解决方案（专注于企业业务的部门）及其母公司联想在商业和企业移动市场占有重要地位，设备安全是该市场的关键卖点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.webpronews.com/grapheneos-expands-to-snapdragon-devices-via-oem-partnership-by-2026/">GrapheneOS Expands to Snapdragon Devices via OEM Partnership by 2026</a></li>
<li><a href="https://reclaimthenet.org/grapheneos-expands-beyond-pixel-phones-with-new-android-partner">GrapheneOS Plans Partnership with Major Android OEM to Expand Beyond ...</a></li>
<li><a href="https://www.motorola.com/us/en/thinkshield">Motorola ThinkShield for Mobile Data Security | Motorola US | motorola</a></li>

</ul>
</details>

**标签**: `#mobile-security`, `#privacy`, `#open-source`, `#android`, `#mobile-operating-systems`

---

<a id="item-8"></a>
## [青龙面板遭.fullgc 挖矿木马植入，导致 CPU 占用率飙升至 800%](https://t.me/zaihuapd/39934) ⭐️ 7.0/10

2026 年 2 月 7 日，多名用户发现流行的开源任务调度工具青龙面板被名为.fullgc 的挖矿木马感染，导致服务器 CPU 占用率异常飙升至 800%。该木马通过篡改 config.sh 配置文件实现持久化，并能根据系统架构自动下载恶意程序。 此次攻击针对的是广泛使用的服务器自动化开源工具，对依赖该工具的系统管理员和开发者构成了重大安全风险。该木马的持久化机制及其对暴露于公网的服务器的针对性，表明这是一个复杂的威胁，可能导致受影响组织遭受严重的资源窃取、性能下降和运营成本增加。 安全机构判定该程序属于 SusMiner 恶意软件家族，主要通过连接 XMR（门罗币）矿池进行非法加密货币挖矿。其主要攻击目标是暴露在公网 IPv4 环境下的服务器，建议用户检查/ql/data/db/路径下的隐藏文件。

telegram · zaihuapd · Feb 28, 13:16

**背景**: 青龙面板（GitHub: whyour/qinglong）是一个支持 Python、JavaScript 和 Shell 脚本的开源定时任务管理平台。它通常通过 Docker 部署，用于自动化执行各种在线任务，例如签到脚本或数据抓取。像此次的.fullgc 变种这样的加密劫持恶意软件，会秘密劫持受害者的计算资源来挖掘加密货币，在未经所有者同意的情况下导致 CPU 使用率飙升。SusMiner 家族是专门为此目的设计的已知恶意软件组。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/whyour/qinglong">GitHub - whyour/ qinglong : 支持 Python3、JavaScript、Shell...</a></li>
<li><a href="https://malpedia.caad.fkie.fraunhofer.de/families">Malware Families</a></li>

</ul>
</details>

**标签**: `#security`, `#malware`, `#server-security`, `#cryptojacking`, `#open-source`

---