---
layout: default
title: "Horizon Summary: 2026-03-31 (ZH)"
date: 2026-03-31
lang: zh
---

> From 24 items, 7 important content pieces were selected

---

1. [Axios npm 包遭入侵，恶意版本投放远程访问木马](#item-1) ⭐️ 9.0/10
2. [谷歌量子 AI 将比特币攻击需求降低 20 倍，或可在 9 分钟内提取私钥](#item-2) ⭐️ 9.0/10
3. [Ollama 为 Apple Silicon 推出 MLX 驱动的推理预览版](#item-3) ⭐️ 8.0/10
4. [阿尔忒弥斯二号任务面临关键隔热罩安全问题](#item-4) ⭐️ 8.0/10
5. [Claude Code 源代码通过 NPM 源码映射文件泄露，暴露反蒸馏防御与产品路线图。](#item-5) ⭐️ 8.0/10
6. [GitHub 出现非官方仓库，从公开 npm 包还原 Claude Code 源代码](#item-6) ⭐️ 8.0/10
7. [美光押注堆叠式 GDDR，最快 2027 年推出样品](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Axios npm 包遭入侵，恶意版本投放远程访问木马](https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan) ⭐️ 9.0/10

2026 年 3 月 31 日，攻击者入侵了一位 Axios 维护者的 npm 账户，并发布了两个恶意版本（v1.14.1 和 v0.30.4）。这些版本注入了一个名为 `plain-crypto-js@4.2.1` 的虚假依赖包，该包通过 postinstall 脚本部署了一个跨平台的远程访问木马。 这是一次影响 JavaScript 生态关键基础设施的重大供应链攻击。Axios 是每周下载量超过 5000 万次的流行 HTTP 客户端库。此次入侵可能导致在安装了恶意包的系统上发生即时凭证窃取，并为攻击者提供持久远程访问，影响无数下游应用和服务。 恶意代码并未直接放在 Axios 源码中，而是隐藏在 `plain-crypto-js` 依赖包的 postinstall 脚本里。攻击利用了先前已被入侵的维护者账户，恶意包于 2026 年 3 月 31 日（UTC）凌晨被快速连续发布。

hackernews · mtud · Mar 31, 02:54

**背景**: npm 是 JavaScript/Node.js 生态默认的软件包注册中心，托管了数百万个可复用的代码库。在此语境下的供应链攻击，是指通过入侵受信任的软件包来注入恶意软件，进而传播到所有依赖该包的应用。远程访问木马是一种能让攻击者控制受感染系统的恶意软件。`postinstall` 脚本是 npm 的一个生命周期钩子，会在包安装后自动运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wiz.io/blog/axios-npm-compromised-in-supply-chain-attack">Axios NPM Distribution Compromised in Supply Chain Attack | Wiz Blog</a></li>
<li><a href="https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan">axios Compromised on npm - Malicious Versions Drop Remote Access Trojan - StepSecurity</a></li>
<li><a href="https://www.sans.org/blog/axios-npm-supply-chain-compromise-malicious-packages-remote-access-trojan">Axios NPM Supply Chain Compromise: Malicious Packages Deliver Remote Access Trojan | SANS Institute</a></li>

</ul>
</details>

**社区讨论**: 社区讨论强调了即时缓解策略，例如设置软件包的最小发布时间（如 7 天）以及在 npm 配置中通过 `ignore-scripts=true` 禁用脚本执行，这些措施本可阻止此次攻击。由于 Axios 的普遍使用，人们对影响的巨大规模表示担忧，并观察到一种重复出现的攻击模式，即利用窃取的凭证入侵更多软件包。部分评论者主张采用“内置电池”式的生态系统，以减少对关键第三方依赖的依赖。

**标签**: `#security`, `#npm`, `#supply-chain`, `#javascript`, `#malware`

---

<a id="item-2"></a>
## [谷歌量子 AI 将比特币攻击需求降低 20 倍，或可在 9 分钟内提取私钥](https://research.google/blog/safeguarding-cryptocurrency-by-disclosing-quantum-vulnerabilities-responsibly/) ⭐️ 9.0/10

谷歌量子 AI 团队发布白皮书，展示通过优化 Shor 算法电路，将破解比特币椭圆曲线加密所需的量子计算资源降低了 20 倍。他们的攻击电路仅需不到 1200-1450 个逻辑量子比特（由不到 50 万个物理量子比特构建），可能在交易广播后约 9 分钟内提取出私钥。 这标志着量子脆弱性评估的范式转变，表明对加密货币钱包的实际攻击可能以远低于先前估计的量子资源实现可行性。大约 690 万枚比特币（约占总供应量的三分之一）因其公钥已暴露在区块链上面临潜在风险，而 2021 年的 Taproot 升级可能进一步扩大这一脆弱钱包的范围。 该团队编译了两套攻击电路，分别需要不到 1200 个和不到 1450 个逻辑量子比特，可在拥有不到 50 万个物理量子比特的超导量子计算机上运行。攻击者可以提前完成大部分准备计算，然后在交易广播后约 9 分钟内提取私钥，这使他们有约 41%的概率在交易确认前窃取资金（考虑到比特币约 10 分钟的出块时间）。

telegram · zaihuapd · Mar 31, 08:03

**背景**: 比特币和以太坊目前依赖椭圆曲线加密（ECC），特别是椭圆曲线数字签名算法（ECDSA）来保护钱包和交易安全。Shor 算法是一种量子计算算法，能高效解决 ECC（和 RSA）背后的数学难题，可能让量子计算机从公钥推导出私钥。逻辑量子比特是由许多脆弱的物理量子比特构建而成的、经过纠错的计算单元，量子纠错对于可靠执行像运行 Shor 算法这样的复杂计算至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://quantumai.google/static/site-assets/downloads/cryptocurrency-whitepaper.pdf">Securing Elliptic Curve Cryptocurrencies against Quantum ...</a></li>
<li><a href="https://www.coindesk.com/tech/2026/03/31/bitcoin-bulls-scramble-for-post-quantum-protection-as-google-drops-bombshell-paper">Bitcoin bulls scramble for post-quantum protection as Google ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Physical_and_logical_qubits">Physical and logical qubits - Wikipedia</a></li>

</ul>
</details>

**标签**: `#quantum-computing`, `#cryptocurrency-security`, `#cryptography`, `#quantum-cryptanalysis`, `#blockchain`

---

<a id="item-3"></a>
## [Ollama 为 Apple Silicon 推出 MLX 驱动的推理预览版](https://ollama.com/blog/mlx) ⭐️ 8.0/10

Ollama 宣布为 Apple Silicon 设备推出 MLX 驱动的推理预览支持，实现了更快速、更高效的本地大语言模型（LLM）执行。此次集成利用了苹果专为 Apple silicon 机器学习设计的 MLX 数组框架。 此次集成显著提升了在 Mac 上本地运行 LLM 的性能和能效，使得设备端 AI 对开发者和用户来说更加实用。它强化了私密、经济高效且不依赖云服务或互联网连接的 AI 应用生态系统。 性能提升在 M5 等新款芯片上尤为显著，基准测试图已表明这一点。该功能目前处于预览阶段，意味着这是稳定版发布前供测试和反馈的早期版本。

hackernews · redundantly · Mar 31, 03:40

**背景**: Ollama 是一个流行的开源工具，可简化在用户计算机上本地运行开源权重大语言模型（LLM）的过程。MLX 是苹果公司创建的一个用于机器学习的数组框架，专为其 Apple silicon 芯片（M1、M2、M3、M4、M5）优化，能够在 GPU 和神经引擎上进行高效计算。使用 Ollama 等工具本地运行模型具有数据隐私、无 API 成本和离线操作等优势，但传统上受限于消费级硬件的计算能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ml-explore/mlx">GitHub - ml-explore/mlx: MLX: An array framework for Apple silicon · GitHub</a></li>
<li><a href="https://aispaces.substack.com/p/the-ultimate-guide-to-running-llms">The Ultimate Guide to Running LLMs Locally with Ollama</a></li>
<li><a href="https://medium.com/data-science-in-your-pocket/apple-m5-chip-apple-wins-the-ultimate-ai-race-0337b97177fa">Apple M5 Chip : Apple wins the ultimate AI race - Medium</a></li>

</ul>
</details>

**社区讨论**: 社区强烈支持向设备端 LLM 发展的趋势，强调了增强隐私性、无需连接或令牌成本以及降低能耗等好处。评论也揭示了实际考量，例如用户寻求经济实惠的本地编码设备，并赞扬了像 OMLX 这样具有 SSD KV 缓存等功能以改善工作流程的互补工具。社区普遍认为本地推理是未来，而性能是剩余的关键障碍。

**标签**: `#ollama`, `#mlx`, `#apple-silicon`, `#local-llm`, `#inference`

---

<a id="item-4"></a>
## [阿尔忒弥斯二号任务面临关键隔热罩安全问题](https://idlewords.com/2026/03/artemis_ii_is_not_safe_to_fly.htm) ⭐️ 8.0/10

一份详细分析报告指出，NASA 即将执行的阿尔忒弥斯二号载人登月任务，其猎户座飞船的隔热罩设计存在严重安全隐患，报告将此与航天飞机哥伦比亚号和挑战者号灾难相提并论。这些担忧源于无人测试任务阿尔忒弥斯一号期间观察到的材料侵蚀问题，以及后续修复措施被认为不够充分。 此事至关重要，因为阿尔忒弥斯二号是 NASA 五十多年来的首次载人重返月球任务，若隔热罩在以月球返回速度再入大气层时失效，对宇航员将是灾难性的。这场争论凸显了 NASA 安全文化中工程谨慎性与项目进度压力之间反复出现的紧张关系，对整个阿尔忒弥斯计划及未来的深空探索都有影响。 该隔热罩采用了更新的 Avcoat 烧蚀材料瓦片设计，但对阿尔忒弥斯一号任务后的分析显示，出现了意外的、局部性的炭化和侵蚀模式。尽管 NASA 和承包商洛克希德·马丁公司坚称存在足够的安全裕度，但以 NASA 前工程师兼宇航员 Tommaso P. Camarda 为代表的批评者认为，失效模式尚未被完全理解，对于载人飞行来说风险是不可接受的。

hackernews · idlewords · Mar 31, 02:23

**背景**: 猎户座飞船的隔热罩是一个关键部件，旨在保护乘员舱在从月球高速再入大气层时免受极端高温（超过 2760°C 或 5000°F）的影响。与航天飞机可重复使用的硅瓦系统不同，猎户座使用一种名为 Avcoat 的一次性烧蚀隔热罩，通过炭化和侵蚀将热量带走。航天飞机项目曾遭遇两次灾难性损失（1986 年的挑战者号和 2003 年的哥伦比亚号），部分原因与其热防护系统故障和组织安全文化有关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://phys.org/news/2026-03-shield-safety-stakes-nasa-artemis.html">Heat shield safety concerns raise stakes for NASA's Artemis ...</a></li>
<li><a href="https://arstechnica.com/space/2026/01/nasa-chief-reviews-orion-heat-shield-expresses-full-confidence-in-it-for-artemis-ii/">Is Orion’s heat shield really safe? New NASA chief conducts ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Space_Shuttle_thermal_protection_system">Space Shuttle thermal protection system - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区讨论反映出深切的担忧和历史类比。一位评论者正在准备一场关于系统性失效的哈佛讲座，他将阿尔忒弥斯二号与挑战者号和哥伦比亚号一起列为案例研究，批评了一种持续存在的“破碎的安全文化”。其他人则对风险水平进行了辩论，有人指出一篇更平衡的外部文章显示，大多数 NASA 工程师和宇航员认为它是安全的，而一位怀疑者则质疑为何不沿用阿波罗时代的隔热罩设计，暗示了任务复杂性可能增加或过去只是运气好。

**标签**: `#space-exploration`, `#safety-engineering`, `#systems-failure`, `#risk-management`, `#organizational-culture`

---

<a id="item-5"></a>
## [Claude Code 源代码通过 NPM 源码映射文件泄露，暴露反蒸馏防御与产品路线图。](https://twitter.com/Fried_rice/status/2038894956459290963) ⭐️ 8.0/10

Anthropic 的 Claude Code 工具的完整源代码在其发布的 NPM 包中包含了一个源码映射文件，导致意外暴露。此次泄露揭示了其专有的反蒸馏防御机制，以及代号为 'kairos' 的 '助手模式' 等未发布功能的细节。 这是一起重大的安全事件，暴露了专有的 AI 安全技术和产品战略，可能削弱 Anthropic 的竞争优势和安全态势。它突显了一个关键的软件供应链漏洞，可能影响任何发布 JavaScript 包的公司。 泄露的发生疑似源于 Bun（Anthropic 拥有的 JavaScript 运行时）的一个漏洞，该漏洞导致源码映射在生产构建中被暴露。暴露的代码包含一个 'ANTI_DISTILLATION_CC' 防御机制，该机制会向 API 请求中注入诱饵工具定义，以污染潜在竞争对手模型的训练数据。

hackernews · treexs · Mar 31, 09:00

**背景**: 源码映射是一种将压缩或打包后的 JavaScript 代码映射回其原始源代码的文件，用于辅助开发者调试，通常在生产版本中会被排除。反蒸馏是 AI 公司使用的一种防御技术，旨在防止竞争对手通过抓取 API 输出来提取模型能力用于训练数据。Claude Code 是 Anthropic 为开发者提供的 AI 驱动编码代理工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/gabrielanhaia/claude-codes-entire-source-code-was-just-leaked-via-npm-source-maps-heres-whats-inside-cjo">Claude Code's Entire Source Code Was Just Leaked via npm ...</a></li>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社区讨论**: 社区发现了一个潜在的根源，即 Bun 的一个漏洞错误地在生产构建中暴露了源码映射。评论者分析了暴露的反蒸馏防御机制，并对未发布产品功能的泄露表示担忧，认为这是一次重大的战略损失。此外，还讨论了 Anthropic 的应对措施，指出他们是将易受攻击的包版本标记为弃用，而非直接撤销发布。

**标签**: `#security`, `#ai-safety`, `#source-code-leak`, `#anthropic`, `#npm`

---

<a id="item-6"></a>
## [GitHub 出现非官方仓库，从公开 npm 包还原 Claude Code 源代码](https://github.com/ChinaSiro/claude-code-sourcemap) ⭐️ 8.0/10

一个名为 'claude-code-sourcemap' 的非官方 GitHub 仓库，通过分析公开 npm 包 `@anthropic-ai/claude-code` 中包含的 `cli.js.map` 源映射文件中的 `sourcesContent` 字段，还原出了 Anthropic 公司 Claude Code 2.1.88 版本的 4756 个 TypeScript 源代码文件。 这一事件突显了一个重大的安全疏忽，即敏感的专有源代码在生产构建中被无意暴露。它罕见地提供了对一款主流 AI 编程助手内部架构的详细洞察，这些信息可能被用于安全研究、竞争分析或潜在的恶意目的。 还原的代码包含 1884 个 `.ts` 和 `.tsx` 源文件，涵盖了 CLI 入口、工具、命令、服务、插件、语音交互和 Vim 模式等模块。仓库维护者明确警告用户不要尝试让 Claude Code 连接此仓库，因为源代码中包含的远程 URL 哈希值可能导致账户安全风险。

telegram · zaihuapd · Mar 31, 09:33

**背景**: 源映射（Source Map）是一种文件，用于将经过压缩或转译（如从 TypeScript 转译）的 JavaScript 代码映射回其原始源代码，以辅助调试。可选的 `sourcesContent` 字段可以将完整的原始源代码直接嵌入到映射文件中。虽然这为调试提供了便利，但在公开发布的生产版本包中包含 `sourcesContent` 字段存在安全风险，因为它相当于公开了原始的、未混淆的源代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.openreplay.com/source-maps-work/">What Are Source Maps and How Do They Work - blog.openreplay.com</a></li>
<li><a href="https://stackoverflow.com/questions/19802462/do-source-maps-include-the-source-text">Do source maps include the source text? - Stack Overflow</a></li>

</ul>
</details>

**标签**: `#reverse-engineering`, `#source-code`, `#ai-tools`, `#security`, `#anthropic`

---

<a id="item-7"></a>
## [美光押注堆叠式 GDDR，最快 2027 年推出样品](https://www.etnews.com/20260330000228) ⭐️ 7.0/10

美光已启动堆叠式 GDDR 内存的研发，计划在 2026 年下半年完成设备部署并进入工艺测试，最快在 2027 年推出约 4 层堆叠的样品。 此举意义重大，因为它旨在打造一个介于高成本的 HBM 和标准 GDDR 之间的全新内存层级，有望为 AI 加速器和 GPU 提供更具成本效益的高带宽解决方案，从而抢占新兴细分市场。 该产品面临芯片互联、功耗、散热以及堆叠工艺带来的成本控制等重大技术挑战。值得注意的是，竞争对手三星电子和 SK 海力士尚未公开类似的计划。

telegram · zaihuapd · Mar 31, 00:36

**背景**: GDDR（图形双倍数据速率内存）和 HBM（高带宽内存）是用于 GPU 和加速器的两种主要高性能内存技术。传统 GDDR 采用 2D 分立芯片设计，而 HBM 则采用 3D 堆叠和硅通孔 (TSV) 技术，以实现更高的带宽和密度，但成本也显著更高。堆叠式 GDDR 旨在融合 GDDR 的成本结构和 3D 堆叠的部分性能优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1936817919486034471">GDDR 和 HBM 的对比 - 知乎</a></li>
<li><a href="https://blog.csdn.net/sinat_37574187/article/details/149797636">HBM vs GDDR有什么异同和优劣 - CSDN博客</a></li>
<li><a href="https://ee.ofweek.com/2025-03/ART-8420-2800-30658974.html">面向高性能的3D-IC芯片堆叠技术，如何普及？——技术现状、挑战与未来前...</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#memory`, `#ai-hardware`, `#gpu`, `#manufacturing`

---