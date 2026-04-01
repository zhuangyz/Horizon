---
layout: default
title: "Horizon Summary: 2026-04-01 (ZH)"
date: 2026-04-01
lang: zh
---

> From 26 items, 6 important content pieces were selected

---

1. [OpenAI 以 8520 亿美元估值完成 1220 亿美元融资轮](#item-1) ⭐️ 9.0/10
2. [供应链攻击通过恶意依赖包入侵 Axios npm 包](#item-2) ⭐️ 9.0/10
3. [Axios npm 维护者账号遭劫持，恶意版本投放远程访问木马](#item-3) ⭐️ 9.0/10
4. [谷歌量子 AI 将比特币攻击门槛降低 20 倍，或可在 9 分钟内提取私钥](#item-4) ⭐️ 9.0/10
5. [Claude Code 源代码泄露揭示隐藏 AI 归属的 '卧底模式'](#item-5) ⭐️ 8.0/10
6. [GitHub 出现非官方仓库，从公开 npm 包还原 Claude Code 的 TypeScript 源码](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 以 8520 亿美元估值完成 1220 亿美元融资轮](https://www.cnbc.com/2026/03/31/openai-funding-round-ipo.html) ⭐️ 9.0/10

OpenAI 宣布完成最新一轮融资，以 8520 亿美元投后估值筹集了 1220 亿美元的承诺资本。这标志着人工智能公司估值的一个历史性里程碑。 这一估值表明市场对 OpenAI 的潜力抱有巨大信心，并标志着人工智能行业估值方式的范式转变。它为该公司提供了前所未有的资本，以加速发展并在快速演变的人工智能格局中竞争。 这笔资金被描述为“承诺资本”，这意味着它可能取决于未来的里程碑，而非立即可用的现金。OpenAI 报告的收入约为每月 20 亿美元，但这一数字的计算方式与 Anthropic 等竞争对手不同，因为 OpenAI 从 Azure 销售中抽取 20%的收入份额。

hackernews · surprisetalk · Mar 31, 20:07

**背景**: OpenAI 是一家领先的人工智能研究和部署公司，以创建 GPT-4 和广泛使用的 ChatGPT 等模型而闻名。融资轮是公司从投资者那里筹集资金以换取股权的过程，“投后估值”是指新投资加入后公司的估计价值。近年来，随着人工智能技术的商业潜力日益清晰，AI 公司的估值大幅飙升。

**社区讨论**: 社区讨论揭示了人们对融资结构的怀疑，用户指出“承诺资本”一词意味着有条件的承诺，而非立即可用的现金。关于收入增长也存在争论，与 Anthropic 的比较突显了不同的收入报告方法。一些人对估值的巨大规模以及公众投资渠道有限表示担忧，而另一些人则将强调 ChatGPT 消费者覆盖范围解读为应对企业市场竞争压力的举措。

**标签**: `#AI`, `#Venture Capital`, `#OpenAI`, `#Business`, `#Valuation`

---

<a id="item-2"></a>
## [供应链攻击通过恶意依赖包入侵 Axios npm 包](https://simonwillison.net/2026/Mar/31/supply-chain-attack-on-axios/#atom-everything) ⭐️ 9.0/10

一次供应链攻击入侵了流行的 HTTP 客户端库 Axios 的 npm 包，具体版本为 1.14.1 和 0.30.4，攻击方式是为其添加了一个名为 plain-crypto-js 的恶意依赖。这个新发布的恶意软件旨在窃取凭证并安装远程访问木马。 这次攻击影响重大，因为 Axios 是一个基础性的 JavaScript 库，每周下载量超过 1.01 亿次，这意味着对整个软件生态系统的潜在影响是巨大的。它突显了广泛使用的开源软件包在供应链攻击面前的极端脆弱性，并强调了采用更安全的发布实践的紧迫性。 这次攻击似乎源于一个泄露的、长期有效的 npm 认证令牌。一个值得注意的检测线索是，这些恶意软件包是在没有伴随 GitHub 发布的情况下发布的，这种模式在最近对 LiteLLM 软件包的攻击中也出现过。

rss · Simon Willison · Mar 31, 23:28

**背景**: 软件供应链攻击是指将恶意代码注入合法的软件组件，从而感染所有依赖该组件的应用程序。npm 是 Node.js JavaScript 运行时的默认包管理器，托管着数百万个开源软件包。可信发布是一项现代安全功能，它取代了传统的基于令牌的认证方式，通常使用 OpenID Connect (OIDC) 等机制来确保软件包只能从授权的自动化工作流（如 GitHub Actions）发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack - Wikipedia</a></li>
<li><a href="https://docs.npmjs.com/about-access-tokens">About access tokens - npm Docs</a></li>
<li><a href="https://docs.npmjs.com/packages-and-modules/contributing-packages-to-the-registry/">Contributing packages to the registry | npm Docs</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain`, `#npm`, `#axios`, `#malware`

---

<a id="item-3"></a>
## [Axios npm 维护者账号遭劫持，恶意版本投放远程访问木马](https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan) ⭐️ 9.0/10

2026 年 3 月 31 日，主流 JavaScript 库 axios 的 npm 维护者账号遭劫持。攻击者绕过了正常的 GitHub Actions CI/CD 流程，手动发布了两个恶意版本：axios@1.14.1 和 axios@0.30.4。这些版本通过引入恶意依赖 plain-crypto-js 来执行脚本，在 Windows、macOS 和 Linux 系统上部署远程访问木马（RAT），并连接到特定的 C2 服务器。 这是一次针对基础 JavaScript 库的重大供应链攻击，该库每周下载量超过 3 亿次，对数以万计的应用程序和开发者构成了巨大风险。此次攻击手法复杂，绕过了自动化安全检查并针对多个操作系统，凸显了开源生态系统中凭证泄露威胁的日益增长。 该恶意软件具有极强的隐蔽性，在执行后会自动删除恶意脚本并伪造干净的配置文件以规避安全审计。恶意依赖 `plain-crypto-js@4.2.1` 被固定在一个在 axios 发布时尚未上传的版本号上，这是一种规避扫描器的策略，因为在恶意包实际发布之前，扫描器不会发现任何异常。

telegram · zaihuapd · Mar 31, 04:10

**背景**: Axios 是一个广泛使用的、基于 Promise 的 JavaScript HTTP 客户端，常用于 Node.js 和浏览器环境中发起网络请求。软件供应链攻击是指攻击者入侵一个被许多下游项目信任和使用的组件、工具或服务，从而间接分发恶意软件。npm（Node Package Manager）registry 是 JavaScript 包的主要仓库，其账户劫持事件会产生连锁的安全影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/axios-npm-compromised-maintainer-hijacked-rat">axios compromised on npm: maintainer account hijacked, RAT deployed</a></li>
<li><a href="https://www.wiz.io/blog/axios-npm-compromised-in-supply-chain-attack">Axios NPM Distribution Compromised in Supply Chain Attack | Wiz Blog</a></li>
<li><a href="https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan">axios Compromised on npm - Malicious Versions Drop Remote Access Trojan - StepSecurity</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain-attack`, `#npm`, `#javascript`, `#malware`

---

<a id="item-4"></a>
## [谷歌量子 AI 将比特币攻击门槛降低 20 倍，或可在 9 分钟内提取私钥](https://research.google/blog/safeguarding-cryptocurrency-by-disclosing-quantum-vulnerabilities-responsibly/) ⭐️ 9.0/10

谷歌量子 AI 团队发布论文，展示了对破解比特币椭圆曲线加密所需量子计算资源的重大优化，将需求降低了约 20 倍。他们编译了两套攻击电路，分别需要不到 1200 个和不到 1450 个逻辑量子比特，这可能在交易广播后约 9 分钟内实现私钥提取。 这标志着量子脆弱性评估的范式转变，大幅缩短了对加密货币发起实际攻击的预估时间线。它凸显了加密生态系统向抗量子算法过渡的紧迫性，因为约有 690 万枚 BTC（占总供应量的三分之一）因公钥暴露而面临潜在风险。 优化后的 Shor 算法电路可在拥有不到 50 万个物理量子比特的超导量子计算机上运行，而此前的估计约为 1000 万个。攻击者在交易确认前（比特币约 10 分钟的出块时间内）窃取资金的成功率约为 41%，其中网络早期钱包（约 170 万枚 BTC）尤其脆弱。

telegram · zaihuapd · Mar 31, 08:03

**背景**: 比特币的安全依赖于椭圆曲线密码学（ECC），私钥用于生成公钥和地址。Shor 算法是一种量子算法，它能以比经典计算机指数级更快的速度解决支撑该密码学的数学问题（如 ECC 的离散对数问题）。逻辑量子比特是由许多易受退相干和错误影响的物理量子比特（基本硬件组件）通过纠错构建而成的计算单元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Shor's_algorithm">Shor's algorithm - Wikipedia</a></li>
<li><a href="https://quantumai.google/static/site-assets/downloads/cryptocurrency-whitepaper.pdf">Securing Elliptic Curve Cryptocurrencies against Quantum ...</a></li>
<li><a href="https://www.forbes.com/sites/digital-assets/2026/03/31/google-finds-quantum-computers-could-break-bitcoin-sooner-than-expected/">Google Finds Quantum Computers Could Break Bitcoin Sooner ...</a></li>

</ul>
</details>

**标签**: `#quantum-computing`, `#cryptocurrency-security`, `#cryptography`, `#blockchain`, `#quantum-cryptanalysis`

---

<a id="item-5"></a>
## [Claude Code 源代码泄露揭示隐藏 AI 归属的 '卧底模式'](https://alex000kim.com/posts/2026-03-31-claude-code-source-leak/) ⭐️ 8.0/10

Anthropic 的 Claude Code 工具的完整 512,000 行 TypeScript 源代码，通过其公开 npm 包中包含的一个 source map 文件被意外泄露。泄露的代码揭示了内部实践，包括一个旨在防止 AI 在提交信息和 PR 描述中暴露其身份的 '卧底模式'。 此次泄露暴露了一家主要 AI 公司开发工具的内部机制和战略实践，引发了关于 AI 透明度、软件开发中的归属伦理以及企业安全实践的严重问题。它还凸显了使用 AI 协助开源贡献与希望隐藏这种协助之间的紧张关系。 泄露发生是因为一个用于调试的 59.8 MB `.map` source map 文件被包含在 `@anthropic-ai/claude-code` npm 包的 2.1.88 版本中。'卧底模式' 明确指示 AI 永远不要在提交中包含 'Claude Code' 或 'Co-Authored-By: Claude' 等短语，从而有效隐藏 AI 生成代码的归属。

hackernews · alex000kim · Mar 31, 13:04

**背景**: Claude Code 是 Anthropic 开发的一款 AI 驱动的编码助手工具。source map 文件是一种调试辅助工具，它将压缩/转译后的代码映射回其原始源代码；如果包含在公开发布版本中，就可能暴露原始源代码。此次泄露发生在另一起 Anthropic 'Mythos' 模型细节被意外暴露的事件之后。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibtimes.co.uk/claude-code-leak-advanced-ai-secrets-1789623">Anthropic Claude Code Leak Reveals Secrets—Self-Healing ...</a></li>
<li><a href="https://dev.to/gabrielanhaia/claude-codes-entire-source-code-was-just-leaked-via-npm-source-maps-heres-whats-inside-cjo">Claude Code's Entire Source Code Was Just Leaked via npm ...</a></li>
<li><a href="https://venturebeat.com/technology/claude-codes-source-code-appears-to-have-leaked-heres-what-we-know">Claude Code's source code appears to have leaked: here's what ...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示出高度参与，辩论集中在 '卧底模式' 的伦理问题、Anthropic 对相关 GitHub 分支的激进 DMCA 下架，以及对一系列安全漏洞模式的担忧。一些评论者对代码中公开注释的内部 '商业机密' 和业务背景的程度感到惊讶，而另一些人则质疑这对用户信任的影响。

**标签**: `#ai-ethics`, `#source-code-leak`, `#software-development`, `#anthropic`, `#security`

---

<a id="item-6"></a>
## [GitHub 出现非官方仓库，从公开 npm 包还原 Claude Code 的 TypeScript 源码](https://github.com/ChinaSiro/claude-code-sourcemap) ⭐️ 8.0/10

一个名为 'claude-code-sourcemap' 的非官方 GitHub 仓库，通过解析公开 npm 包 `@anthropic-ai/claude-code` 中包含的 source map 文件 `cli.js.map` 中的 `sourcesContent` 字段，成功还原了 Anthropic 旗下 Claude Code 2.1.88 版本的 TypeScript 源代码，共计 4756 个文件，其中包括 1884 个 `.ts` 与 `.tsx` 源文件。还原的目录涵盖了 CLI 入口、工具、命令、服务、插件、语音交互和 Vim 模式等模块。 这一事件凸显了一个重大的安全疏忽：敏感的商业源代码可能通过生产环境 npm 包中包含的 source map 等调试工件被无意中暴露。这为所有工程团队敲响了警钟，必须审计其构建和部署流程，以防止无意的源代码泄露，这种泄露可能帮助竞争对手或恶意行为者理解并可能利用软件的架构。 仓库说明明确指出，还原内容基于公开发布的包和 source map 分析整理，不代表官方的原始内部开发仓库结构，仅供研究使用。仓库页面包含显著警告，提醒用户不要试图让 Claude Code 链接此仓库，因为上报信息中包含的 remote url 的 hash 可能导致账户风险。

telegram · zaihuapd · Mar 31, 09:33

**背景**: Source map 是一种将压缩或转译后的代码（如 JavaScript）映射回其原始源代码（如 TypeScript）的文件，主要用于在浏览器开发者工具中辅助调试。它们通常包含一个 `sourcesContent` 字段，该字段可以嵌入完整的原始源代码。当此类 source map 文件被包含在公开发布的 npm 包中时，它们可被用于逆向工程并重建原始的可读源代码，如果在生产构建过程中未正确移除，实质上就造成了代码库的泄露。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/gabrielanhaia/claude-codes-entire-source-code-was-just-leaked-via-npm-source-maps-heres-whats-inside-cjo">Claude Code's Entire Source Code Was Just Leaked via npm ...</a></li>
<li><a href="https://stackoverflow.com/questions/32383865/how-to-use-sourcemaps-to-restore-the-original-file">javascript - How to use sourcemaps to restore the... - Stack Overflow</a></li>
<li><a href="https://wellstsai.com/en/post/restoring-source-code-from-sourcemaps/">Restoring Frontend Source Code Using Sourcemaps: Practical ...</a></li>

</ul>
</details>

**标签**: `#reverse-engineering`, `#source-maps`, `#anthropic`, `#claude`, `#security`

---