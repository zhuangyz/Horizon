---
layout: default
title: "Horizon Summary: 2026-03-15 (ZH)"
date: 2026-03-15
lang: zh
---

> From 20 items, 6 important content pieces were selected

---

1. [科学家实现成年小鼠大脑玻璃化冷冻及功能恢复](#item-1) ⭐️ 9.0/10
2. [Jazzband Python 项目因 AI 生成的垃圾 PR 而关闭](#item-2) ⭐️ 8.0/10
3. [Glassworm 攻击利用不可见 Unicode 字符入侵逾 151 个 GitHub 仓库](#item-3) ⭐️ 8.0/10
4. [苹果发布采用全新 Fusion Architecture 的 M5、M5 Pro 和 M5 Max 芯片](#item-4) ⭐️ 8.0/10
5. [Simon Willison 在 Pragmatic Summit 上讨论智能体工程与 AI 采用阶段](#item-5) ⭐️ 7.0/10
6. [NASA 监察机构警告阿耳忒弥斯计划缺乏月面救援能力且着陆器存在技术隐患](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [科学家实现成年小鼠大脑玻璃化冷冻及功能恢复](https://www.pnas.org/doi/10.1073/pnas.2516848123) ⭐️ 9.0/10

研究人员在《美国国家科学院院刊》（PNAS）上发表成果，成功对成年小鼠脑片及原位全脑进行了玻璃化冷冻，并在复温后恢复了其神经功能。该团队开发了名为 V3 的玻璃化保护剂溶液，并通过优化冷却流程有效避免了冰晶损伤，使组织能在低于玻璃化转变温度的环境下稳定保存。 这是低温生物学和神经科学领域的一项重大突破，首次证明复杂的成年哺乳动物脑组织可以被玻璃化冷冻，并在复温后保留功能性神经活动和突触可塑性。这为保存具有完整功能结构的脑组织开辟了新途径，对神经科学研究、脑库建设以及未来医疗技术具有深远的潜在影响。 实验结果显示，复温后的脑片恢复了细胞代谢，并保持了电生理活性及突触可塑性。在全脑保存方面，研究者通过血管灌注技术平衡了脱水与保护剂渗透，初步实现了原位全脑的冷冻与功能保留。

telegram · zaihuapd · Mar 15, 08:30

**背景**: 玻璃化冷冻是一种低温保存技术，通过快速冷却使生物样本形成一种无定形的、玻璃状的固体，从而避免传统慢速冷冻过程中形成的破坏性冰晶。冷冻保护剂是添加到生物样本中以保护细胞免受冷冻损伤的化学物质。玻璃化转变温度是一个临界点，低于此温度材料会进入稳定的玻璃态，这对长期保存至关重要。血管灌注是一种通过器官循环系统均匀输送冷冻保护剂的方法，由于血脑屏障的存在，这对大脑来说尤其具有挑战性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vitrification">Vitrification - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11753176/">Cryopreservation of brain cell structure: a review - PMC</a></li>

</ul>
</details>

**标签**: `#cryobiology`, `#neuroscience`, `#vitrification`, `#brain-preservation`, `#PNAS`

---

<a id="item-2"></a>
## [Jazzband Python 项目因 AI 生成的垃圾 PR 而关闭](https://simonwillison.net/2026/Mar/14/jannis-leidel/#atom-everything) ⭐️ 8.0/10

Jazzband 开源社区于 2026 年 3 月 14 日宣布将逐步停止运营。这一决定是由于 GitHub 的'垃圾泛滥'——即大量 AI 生成的垃圾拉取请求和问题——使其开放的成员资格和共享推送权限模式变得不可持续。 这次关闭事件凸显了依赖开放协作的开源项目在可持续性方面面临的系统性威胁。它表明 AI 生成的垃圾内容正迫使项目放弃包容性模式，这可能会减少社区贡献，并加剧整个生态系统中维护者的倦怠。 Jazzband 引用了具体数据：只有十分之一的 AI 生成 PR 符合项目标准，而 curl 项目因其漏洞悬赏计划的确认率降至 5%以下而不得不关闭该计划。GitHub 自身的应对措施包括引入一个'紧急开关'，以便为受影响的仓库完全禁用拉取请求功能。

rss · Simon Willison · Mar 14, 18:41

**背景**: Jazzband 是一个维护基于 Python 项目的开放社区，其运作模式是任何成员都可以获得对代码库的推送权限。'垃圾泛滥'一词指的是大量低质量、AI 生成的内容（如拉取请求和问题）淹没平台的现象。这一现象已成为开源维护者的主要痛点，迫使他们花费过多时间过滤垃圾信息，而非进行生产性工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jazzband.co/">Jazzband - We are all part of this</a></li>
<li><a href="https://unprecedented.ghost.io/archive/the-ai-slopocalypse/">The AI Slopocalypse</a></li>
<li><a href="https://prevhq.com/blog/the-open-source-spam-apocalypse">The Open Source Spam Apocalypse (And How to Survive It)</a></li>

</ul>
</details>

**标签**: `#open-source`, `#ai-spam`, `#github`, `#maintenance`, `#sustainability`

---

<a id="item-3"></a>
## [Glassworm 攻击利用不可见 Unicode 字符入侵逾 151 个 GitHub 仓库](https://www.tomshardware.com/tech-industry/cyber-security/malicious-packages-using-invisible-unicode-found-in-151-github-repos-and-vs-code) ⭐️ 8.0/10

Aikido Security 的研究人员发现，名为 Glassworm 的黑客组织利用不可见的 Unicode 字符（特别是零宽空格）在代码中隐藏恶意负载。该攻击已确认入侵至少 151 个 GitHub 仓库、npm 包和 VS Code 扩展，包括 Wasmer 和 Reworm 等知名项目。 此次攻击之所以重要，是因为它利用了人工代码审查过程中的一个根本性弱点，使得恶意代码对开发者几乎不可见。这是一次复杂的软件供应链攻击，能够窃取用户凭据和加密代币，可能影响所有使用这些被入侵开源项目的下游用户。 恶意负载旨在窃取用户凭据和加密代币，攻击者还利用 Solana 区块链作为指令控制通道，增加了关停难度。研究人员指出，攻击者疑似利用大语言模型生成了与各目标项目风格一致的代码重构和版本更新，从而增强了欺骗性。

telegram · zaihuapd · Mar 15, 01:28

**背景**: 零宽 Unicode 字符（如 U+200B 零宽空格）是不可见的非打印字符，在文本中渲染为空白。它们本用于文本格式化，但在网络安全领域可能被滥用于制造同形异义字攻击或隐藏恶意代码，因为人工审查者难以察觉。软件供应链攻击通过入侵软件依赖项（如 npm 包）来危害大量下游应用程序。Solana 是一个支持智能合约和去中心化应用的高性能区块链平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-width_space">Zero-width space - Wikipedia</a></li>
<li><a href="https://www.promptfoo.dev/blog/invisible-unicode-threats/">The Invisible Threat: How Zero-Width Unicode Characters Can Silently Backdoor Your AI-Generated Code | Promptfoo</a></li>
<li><a href="https://www.cisa.gov/news-events/alerts/2025/09/23/widespread-supply-chain-compromise-impacting-npm-ecosystem">Widespread Supply Chain Compromise Impacting npm Ecosystem</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#supply-chain-attack`, `#unicode`, `#github`, `#npm`

---

<a id="item-4"></a>
## [苹果发布采用全新 Fusion Architecture 的 M5、M5 Pro 和 M5 Max 芯片](https://t.me/zaihuapd/40272) ⭐️ 8.0/10

苹果宣布了其下一代 M5 系列芯片，包括 M5、M5 Pro 和 M5 Max，其采用了全新的 'Fusion Architecture' 设计，将两个芯片组合成一个单一的系统级芯片。M5 Pro 和 M5 Max 配备了 18 核 CPU，包括 6 个 '超级核心' 和 12 个 '性能核心'，承诺为专业工作负载带来显著的性能提升。 这标志着苹果自研芯片的一次重大架构转变，从单片式设计转向多芯片的 'Fusion' 设计，这可能为高端 MacBook Pro 型号带来更强的可扩展性、性能和能效。新的核心命名方案和宣称的性能飞跃，进一步强化了苹果凭借其定制芯片主导专业笔记本电脑市场的战略。 新的 '超级核心' 似乎是上一代性能核心的重命名，而新的 '性能核心' 很可能是改进后的能效核心，从而形成了一个三层的 CPU 核心层级。Fusion Architecture 标志着苹果脱离了传统的单片式 SoC 设计，可能有助于实现更专业化的核心配置和更高的核心数量。

telegram · zaihuapd · Mar 15, 07:20

**背景**: Apple Silicon 是指苹果为其 Mac 电脑设计的自研系统级芯片系列，它将 CPU、GPU、内存和其他组件集成到单一芯片上，以实现高性能和高能效。在 M5 之前，苹果的芯片采用统一架构，包含两种类型的 CPU 核心：高性能的 'P-核心' 和高能效的 'E-核心'，所有核心都制造在单片硅晶圆上。系统级芯片是一种集成电路，它将计算机或电子系统的全部或大部分组件（如处理器、内存和输入/输出端口）整合到单一芯片中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/tyson_cung/apple-m5-fusion-architecture-explained-two-dies-one-chip-infinite-possibilities-o9e">Apple M5 Fusion Architecture Explained - Two... - DEV Community</a></li>
<li><a href="https://www.macworld.com/article/3077260/what-the-hell-is-an-m5-super-core.html">M5 deep dive: What the hell is a super core? | Macworld</a></li>
<li><a href="https://en.wikipedia.org/wiki/System_on_a_chip">System on a chip - Wikipedia</a></li>

</ul>
</details>

**标签**: `#apple-silicon`, `#hardware`, `#macbook`, `#soc`, `#performance`

---

<a id="item-5"></a>
## [Simon Willison 在 Pragmatic Summit 上讨论智能体工程与 AI 采用阶段](https://simonwillison.net/2026/Mar/14/pragmatic-summit/#atom-everything) ⭐️ 7.0/10

Simon Willison 分享了他在旧金山 Pragmatic Summit 上炉边谈话的要点，其中概述了开发者采用 AI 的不同阶段，并讨论了智能体工程的实用模式。他特别提到，大约六个月前，他进入了 AI 智能体编写的代码比他本人更多的阶段，并阐述了他目前如何与智能体一起使用测试驱动开发（TDD）。 这次讨论为开发者应对向 AI 辅助编程的转变提供了一个具体框架，既揭示了其中的潜力，也指出了关键的信任挑战。随着 StrongDM 等公司向全自动的“软件工厂”迈进，理解这些采用模式和负责任的做法对于软件开发的未来至关重要。 Willison 强调，与智能体一起使用红绿测试驱动开发（例如，通过指示它们“使用红绿 TDD”）能显著提高获得可用代码的几率。他还指出，Opus 4.5 是第一个在特定他已充分理解的问题类别（如构建 JSON API）上赢得他信任的 AI 模型。

rss · Simon Willison · Mar 14, 18:19

**背景**: 智能体工程指的是有效使用 AI 编码智能体的模式和实践，其中智能体在生成甚至执行代码方面扮演主动角色。Pragmatic Summit 是由 Gergely Orosz 和 The Pragmatic Engineer 主办的一日会议，专注于实用的工程主题。主持这次谈话的 Statsig 代表来自一家提供实验和功能管理工具的产品开发平台，该公司近期估值达 11 亿美元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Feb/23/agentic-engineering-patterns/">Writing about Agentic Engineering Patterns</a></li>
<li><a href="https://www.pragmaticsummit.com/">The Pragmatic Summit</a></li>
<li><a href="https://statsig.com/">Statsig | The modern product development platform</a></li>

</ul>
</details>

**标签**: `#AI`, `#Agentic Engineering`, `#Developer Tools`, `#AI Adoption`

---

<a id="item-6"></a>
## [NASA 监察机构警告阿耳忒弥斯计划缺乏月面救援能力且着陆器存在技术隐患](https://futurism.com/space/nasa-oig-rescue-lunar-astronauts-emergency) ⭐️ 7.0/10

NASA 监察长办公室（OIG）于 2026 年 3 月发布的报告披露，阿耳忒弥斯计划已“排除”为早期载人任务中可能被困月球的宇航员开发紧急救援能力。报告还指出了 SpaceX 星舰载人着陆系统（HLS）的重大技术风险，包括其至少需要 10 次燃料加注任务、着陆时倾斜耐受度有限，以及用于宇航员出入的唯一电梯系统存在单点故障风险。 这凸显了 NASA 旗舰重返月球计划中存在关键且未缓解的安全漏洞，直接挑战了其载人探索“安全第一”的原则。所发现的商业着陆器风险，特别是 SpaceX 复杂的在轨加注架构和缺乏冗余设计，可能导致关键的阿耳忒弥斯 3 号登月任务进一步延期、成本超支甚至任务失败。 OIG 报告指出，如果着陆器发生灾难性事件，NASA 没有能力从太空或月球表面营救宇航员。对于 SpaceX 的星舰 HLS，具体担忧包括其 171 英尺的高度使其在崎岖的月球南极容易倾覆，以及 115 英尺的电梯是机组人员到达月面的唯一途径，且没有备用的出入方法。

telegram · zaihuapd · Mar 15, 02:09

**背景**: NASA 的阿耳忒弥斯计划旨在让人类重返月球，其中阿耳忒弥斯 3 号任务的目标是在月球南极附近进行载人着陆。该计划严重依赖商业合作伙伴：SpaceX 获得了开发星舰 HLS 的合同，蓝色起源（Blue Origin）也在开发另一种着陆器。星舰 HLS 是 SpaceX 完全可重复使用航天器的一个变体，但其巨大的尺寸要求它在前往月球之前，必须在近地轨道由多艘“加油船”星舰进行燃料加注——这是一项从未在所需规模上演示过的复杂操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://oig.nasa.gov/news/artemis-lander-program-faces-schedule-delays-and-unmitigated-crew-safety-risks/">Artemis Lander Program Faces Schedule Delays and Unmitigated ...</a></li>
<li><a href="https://news.quantosei.com/2026/03/11/nasa-and-spacex-disagree-about-manual-controls-for-lunar-lander/">NASA & SpaceX Battle Over Crucial Lunar Lander Manual Controls - QuantoSei News</a></li>
<li><a href="https://gist.ly/youtube-summarizer/spacex-orbital-refueling-blue-origins-lunar-landers-explained">SpaceX Orbital Refueling & Blue Origin's Lunar Landers Explained</a></li>

</ul>
</details>

**标签**: `#space-exploration`, `#systems-engineering`, `#risk-management`, `#nasa`, `#spacex`

---