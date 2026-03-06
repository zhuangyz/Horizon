---
layout: default
title: "Horizon Summary: 2026-03-06 (ZH)"
date: 2026-03-06
lang: zh
---

> From 27 items, 11 important content pieces were selected

---

1. [OpenAI 发布 GPT-5.4，具备 100 万 token 上下文窗口和具有竞争力的定价。](#item-1) ⭐️ 9.0/10
2. [苹果发布采用全新 Fusion Architecture 的 M5 Pro 和 M5 Max 芯片用于 MacBook Pro，并为 MacBook Air 配备 M5 芯片。](#item-2) ⭐️ 9.0/10
3. [研究论文指出全球变暖已显著加速](#item-3) ⭐️ 8.0/10
4. [System76 反对要求操作系统内置监控功能的年龄验证法律](#item-4) ⭐️ 8.0/10
5. [安全研究员演示通过 GitHub Issue 标题的提示注入攻击，可破坏 Cline 的生产版本发布。](#item-5) ⭐️ 8.0/10
6. [AI 编程助手通过“净室”重写 chardet 库引发开源许可争议](#item-6) ⭐️ 8.0/10
7. [美国拟推全球 AI 芯片出口许可制度，强化对英伟达和 AMD 的管控](#item-7) ⭐️ 8.0/10
8. [Anthropic CEO 紧急重启五角大楼谈判，试图挽回被定性为供应链风险后的 AI 供应协议](#item-8) ⭐️ 8.0/10
9. [荷兰暂停《商品可得性法》干预，将安世半导体控制权归还中国母公司闻泰科技](#item-9) ⭐️ 8.0/10
10. [研究发现近半数第三方大语言模型中转 API 存在模型不一致问题](#item-10) ⭐️ 7.0/10
11. [消息称美国海关与边境保护局可利用广告定位数据进行监控](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI 发布 GPT-5.4，具备 100 万 token 上下文窗口和具有竞争力的定价。](https://openai.com/index/introducing-gpt-5-4/) ⭐️ 9.0/10

OpenAI 宣布了其主要的全新 AI 模型 GPT-5.4，该模型具备 100 万 token 的上下文窗口。其定价为每百万输入 token 2.50 美元，每百万输出 token 15 美元，这比 Claude Opus 4.6 等竞争对手的价格要低得多。 巨大的 100 万 token 上下文窗口使得模型能够一次性处理整本书、长篇研究论文或大型代码库，这可能会减少对复杂检索增强生成（RAG）架构的需求。具有竞争力的定价使开发者和企业更容易获得先进的长上下文 AI 能力，加剧了 LLM 市场的竞争。 与某些模型对超出特定 token 限制的生成收取额外费用不同，GPT-5.4 的定价包含了完整的 100 万上下文窗口，没有额外费用。OpenAI 还为 GPT-5.4 发布了 'Thinking System Card'，详细说明了其安全性和推理能力，该卡片基于 GPT-5.3 Codex 中使用的方法构建。

hackernews · mudkipdev · Mar 5, 18:08

**背景**: 大型语言模型（LLM）中的上下文窗口是指模型在生成响应时一次性能考虑的最大文本量（以 token 计量）。在此次发布之前，许多领先模型（如 Claude Opus）支持的上下文窗口约为 20 万 token，有些则提供扩展的 100 万 token 窗口作为测试版或高级功能。一个 token 大约相当于 3/4 个单词，因此 100 万 token 的窗口可以处理大约 75 万单词的文本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/build-with-claude/context-windows">Context windows - Claude API Docs</a></li>
<li><a href="https://deploymentsafety.openai.com/gpt-5-4-thinking">GPT -5.4 Thinking System Card - OpenAI Deployment Safety Hub</a></li>
<li><a href="https://atlan.com/know/llm-context-window-limitations/">LLM Context Window Limitations: Impacts, Risks, and Fixes</a></li>

</ul>
</details>

**社区讨论**: 社区讨论强调了 GPT-5.4 相对于 Claude Opus 等竞争对手的显著成本优势。用户正在测试其能力，其中一位用户指出，在多智能体编码场景中观察到一个有趣的现象，即模型似乎会不公平地推卸责任。另一位用户指出了公告博客文章的一个讽刺之处：其包含的 'Ask ChatGPT' 功能实际上无法处理博客本身的内容。

**标签**: `#artificial-intelligence`, `#llm`, `#openai`, `#machine-learning`, `#developer-tools`

---

<a id="item-2"></a>
## [苹果发布采用全新 Fusion Architecture 的 M5 Pro 和 M5 Max 芯片用于 MacBook Pro，并为 MacBook Air 配备 M5 芯片。](https://t.me/zaihuapd/40055) ⭐️ 9.0/10

苹果宣布了其下一代 M5 系列芯片，包括为 MacBook Pro 设计的 M5 Pro 和 M5 Max，以及为 MacBook Air 配备的标准 M5 芯片。M5 Pro 和 M5 Max 采用了苹果全新设计的 Fusion Architecture，将两个芯片裸片连接成一个单一 SoC，并配备了 18 核 CPU。 此次发布代表了 Apple Silicon 的一次重大架构转变，有望为笔记本电脑上的高要求专业工作流带来显著的性能提升。全新的 Fusion Architecture 和核心设计可能为专业计算市场的能效和性能树立新标杆，直接影响内容创作者、开发者和其他专业用户。 M5 Pro 和 M5 Max 的 18 核 CPU 包含 6 个‘超级核心’和 12 个性能核心，这种配置表明其设计重点在于平衡高单线程性能与多线程吞吐能力。Fusion Architecture 将两个裸片组合成一个 SoC 的设计是一项关键的技术进步，旨在实现超越传统单片芯片设计的性能扩展。

telegram · zaihuapd · Mar 6, 00:10

**背景**: Apple Silicon 指的是苹果自 2020 年 M1 芯片开始，为其 Mac 电脑设计的一系列基于 ARM 架构的系统级芯片（SoC）和系统级封装（SiP）处理器。这些芯片通常将 CPU（包含性能核心和能效核心）、GPU、神经网络引擎（NPU）和其他组件集成到单一硅片上，以其高能效比著称。从 M1 到 M4 的演进过程中，CPU/GPU 核心、晶体管数量以及高级矩阵扩展（AMX）等专用加速器都得到了迭代改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/03/apple-debuts-m5-pro-and-m5-max-to-supercharge-the-most-demanding-pro-workflows/">Apple debuts M5 Pro and M5 Max to supercharge the most demanding ...</a></li>
<li><a href="https://techcrunch.com/2026/03/03/apple-unveils-m5-pro-and-m5-max-chips-with-new-fusion-architecture/">Apple unveils M5 Pro and M5 Max chips with new ‘Fusion ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_silicon">Apple silicon</a></li>

</ul>
</details>

**标签**: `#apple-silicon`, `#hardware`, `#macbook`, `#computer-architecture`, `#professional-workflow`

---

<a id="item-3"></a>
## [研究论文指出全球变暖已显著加速](https://www.researchgate.net/publication/389855619_Global_Warming_has_Accelerated_Significantly) ⭐️ 8.0/10

一篇发表在 ResearchGate 平台上的新研究论文（可作为开放获取的预印本获取）分析了近期的气候数据，得出结论认为全球变暖的速度已显著增加。该论文的作者是公认的、被高度引用的气候科学家，这增加了研究结果的可信度。 这一发现意义重大，因为变暖加速意味着气候变化的影响——如极端天气、海平面上升和生态系统破坏——将比先前预测的来得更快、更严重。它强调了采取更雄心勃勃的全球气候行动和政策调整以缓解这些不断升级的风险的紧迫性。 该论文是一篇预印本，意味着它尚未在科学期刊上经过正式的同行评审，但作者在该领域的公认声誉已被指出。分析基于近期的观测气候数据，但用于定义“加速”的具体指标和时间范围在提供的信息中未详细说明。

hackernews · morsch · Mar 6, 14:10

**背景**: 全球变暖指的是由于人类活动（主要是二氧化碳等温室气体的排放）导致的地球平均地表温度的长期上升。变暖的速度是气候模型和政策制定的关键指标，因为它决定了未来影响的时间线和严重程度。该领域的研究论文在正式发表前通常需要经过同行评审，以验证其方法和结论。

**社区讨论**: 社区讨论包括对开放获取来源和作者可信度的核实，并提供了原始预印本的链接。讨论情绪反映了担忧和无奈，评论强调了行动面临的地缘政治挑战、由于发展需求而认为变暖持续不可避免的看法，以及对除非直接受到影响否则社会是否愿意解决问题的怀疑。

**标签**: `#climate-science`, `#environment`, `#research`, `#global-warming`, `#sustainability`

---

<a id="item-4"></a>
## [System76 反对要求操作系统内置监控功能的年龄验证法律](https://blog.system76.com/post/system76-on-age-verification/) ⭐️ 8.0/10

硬件制造商兼 Linux 发行商 System76 发表公开声明，反对加州和科罗拉多州提出的年龄验证法律，这些法律要求操作系统内置监控功能。该公司认为这些法律威胁用户隐私，并将育儿责任不恰当地转移给国家和科技公司。 这很重要，因为它代表了一家重要的硬件和开源软件公司公开反对政府在操作系统层面强制要求监控功能。如果此类法律成为标准，可能会从根本上改变用户、其设备与软件提供商之间的关系，并为国家加强对个人计算的控制开创先例。 System76 特别提到，加州的法律以及以其为蓝本的科罗拉多州法律，是与主要的操作系统提供商协商一致的。该公司指出，如果这种年龄证明方法成为标准，当未提供信号时，应用程序和网站将不承担责任，从而将负担转移给操作系统供应商。

hackernews · LorenDB · Mar 6, 04:12

**背景**: System76 是一家设计和制造预装其自有 Linux 发行版 Pop!_OS 的计算机公司。所提及的年龄验证法律旨在限制未成年人访问某些在线内容，但通常提出诸如操作系统级监控等技术实施方案。争论的核心在于如何在保护儿童与用户隐私、数字权利之间取得平衡，以及技术公司相对于父母和国家的适当角色。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/System76">System76 - Wikipedia</a></li>
<li><a href="https://system76.com/about/">About Us - System76</a></li>
<li><a href="https://www.khlaw.com/insights/ftc-issues-coppa-enforcement-policy-statement-promoting-age-verification-technology">FTC COPPA Policy on Age-Verification Tech | Keller and Heckman</a></li>

</ul>
</details>

**社区讨论**: 社区情绪强烈支持 System76 的立场，赞扬该公司在隐私问题上表明立场。主要观点包括：强烈反对将育儿责任转移给国家和公司的法律；批评一些人认为根植于文化禁欲主义的“保姆国家”越权行为；以及认为过度保护儿童可能有害，有些人主张采用更渐进的、欧洲风格的方式来赋予自主权。

**标签**: `#privacy`, `#government-regulation`, `#linux`, `#digital-rights`, `#corporate-policy`

---

<a id="item-5"></a>
## [安全研究员演示通过 GitHub Issue 标题的提示注入攻击，可破坏 Cline 的生产版本发布。](https://simonwillison.net/2026/Mar/6/clinejection/#atom-everything) ⭐️ 8.0/10

安全研究员 Adnan Khan 演示了一种新颖的攻击链：通过在 GitHub Issue 标题中进行提示注入，诱骗 Cline 基于 AI 的 Issue 分类系统（使用 anthropics/claude-code-action）执行恶意命令。这导致了缓存污染，最终使攻击者能够向 npm 发布一个被破坏的版本（cline@2.3.0）。 这次攻击揭示了在开发工作流中使用 AI 自动化的项目面临一种新的关键供应链风险，展示了看似孤立的自动化（如 Issue 分类）如何被武器化以破坏生产版本发布。它突显了在集成了具有广泛工具访问权限的强大 AI 代理的 CI/CD 流水线中，共享缓存和沙箱隔离不足所带来的危险。 该攻击利用了 Issue 分类工作流和夜间发布工作流之间共享的 GitHub Actions 缓存密钥，从而实现了缓存污染。研究员的'cacheract'包通过用垃圾数据填充缓存来强制其被驱逐，然后植入窃取密钥的机制。尽管 Issue 分类工作流最初没有 npm 发布密钥，但缓存污染打破了这种隔离。

rss · Simon Willison · Mar 6, 02:39

**背景**: GitHub Actions 是一个 CI/CD 平台，可直接在代码仓库内自动化软件工作流。Claude Code 是 Anthropic 推出的 AI 编码助手，在获得权限后可以执行命令并与 Bash 等工具交互。NPM 供应链攻击是指通过破坏软件依赖项（如 npm 包）来向下游项目注入恶意代码，通常利用安装脚本实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/actions">GitHub Actions documentation - GitHub Docs</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Claude Code overview - Claude Code Docs</a></li>
<li><a href="https://www.uprootsecurity.com/blog/npm-supply-chain-attacks-guide">NPM Supply Chain Attack: What Developers Must Know</a></li>

</ul>
</details>

**标签**: `#security`, `#prompt-injection`, `#ai-automation`, `#github-actions`, `#supply-chain`

---

<a id="item-6"></a>
## [AI 编程助手通过“净室”重写 chardet 库引发开源许可争议](https://simonwillison.net/2026/Mar/5/chardet/#atom-everything) ⭐️ 8.0/10

流行 Python 库 chardet 的维护者发布了 7.0.0 版本，声称这是一个完整的、采用 MIT 许可的重写，可作为直接替代品。原始作者 Mark Pilgrim 立即提出异议，认为维护者长期接触原 LGPL 许可的代码，因此无权重新许可，无论其是否为重写。 这一事件凸显了 AI 辅助开发与开源许可交叉领域一个关键且未解决的法律和伦理问题：AI 编程助手能否被用来有效创建法律上独立的、现有代码的“净室”实现，以绕过 LGPL 等限制性许可。其结果可能为 AI 时代如何定义衍生作品开创先例，潜在地影响无数开源项目及其治理。 维护者 Dan Blanchard 使用 JPlag 抄袭检测工具来论证新代码在结构上是独立的，与前一版本仅显示 1.29% 的相似度，与 1.1 版本仅 0.64%。这与传统的净室流程形成对比，后者依赖团队的严格隔离来避免版权污染，而 Blanchard 作为长期维护者，这种隔离并不存在。

rss · Simon Willison · Mar 5, 16:49

**背景**: “净室”实现是一种软件开发方法，由一个团队分析系统以创建规范，再由另一个完全隔离、未接触过原始代码的团队从头开始实现。这是一种在不侵犯版权的情况下创建兼容产品的法律策略，著名的例子是 Compaq 在 1982 年克隆 IBM BIOS。LGPL（GNU 宽通用公共许可证）是一种著佐权（copyleft）许可，要求对原始库的修改必须以相同许可发布，但它允许与非 LGPL 代码链接。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cleanroom_software_engineering">Cleanroom software engineering - Wikipedia</a></li>
<li><a href="https://www.law.cornell.edu/wex/clean_room">clean room | Wex | US Law | LII / Legal Information Institute</a></li>

</ul>
</details>

**标签**: `#AI-coding-agents`, `#open-source-licensing`, `#software-ethics`, `#clean-room-implementation`, `#legal-issues`

---

<a id="item-7"></a>
## [美国拟推全球 AI 芯片出口许可制度，强化对英伟达和 AMD 的管控](https://techcrunch.com/2026/03/05/us-reportedly-considering-sweeping-new-chip-export-controls/) ⭐️ 8.0/10

美国商务部已拟定新规草案，要求美国企业向境外任何地区出口 AI 芯片均须获得政府许可。据报道，拟议的法规还包括要求外国公司作为出口流程的一部分，对美国的人工智能基础设施进行投资。 这标志着美国从先前针对特定国家（如中国）的管制，升级为近乎全球性的许可制度，可能使美国政府获得对关键 AI 技术跨国流动的前所未有的监督权。此举可能重塑全球 AI 发展时间表、供应链以及英伟达和 AMD 等半导体巨头的竞争格局，同时也旨在吸引资本并加强美国国内 AI 生态系统。 草案提议根据交易规模进行分级审查，小额订单接受基础审查，大额订单则需买方政府参与。此举延续了美国对华芯片出口政策不断演变且时有反复的模式，但新规意在通过对全球 AI 芯片贸易建立持续、全面的控制来实现常态化监管。

telegram · zaihuapd · Mar 6, 01:27

**背景**: 美国越来越多地将先进半导体出口管制作为经济治国和国家安全政策的工具，尤其针对中国的技术发展。美国商务部下属的工业和安全局（BIS）负责执行这些管制，自 2022 年以来管制措施逐步收紧。英伟达和 AMD 等公司设计的高性能图形处理器（GPU）对于训练和运行大型 AI 模型至关重要，这使得它们成为这些监管工作的核心目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reuters.com/world/us-mulls-new-rules-ai-chip-exports-including-requiring-investments-by-foreign-2026-03-05/">US mulls new rules for AI chip exports, including requiring US ...</a></li>
<li><a href="https://techcrunch.com/2026/03/05/us-reportedly-considering-sweeping-new-chip-export-controls/">US reportedly considering sweeping new chip export controls</a></li>
<li><a href="https://www.bis.gov/press-release/department-commerce-revises-license-review-policy-semiconductors-exported-china">US Department of Commerce - Bureau of Industry and Security</a></li>

</ul>
</details>

**标签**: `#AI Policy`, `#Semiconductors`, `#Export Controls`, `#Geopolitics`, `#Nvidia`

---

<a id="item-8"></a>
## [Anthropic CEO 紧急重启五角大楼谈判，试图挽回被定性为供应链风险后的 AI 供应协议](https://t.me/zaihuapd/40062) ⭐️ 8.0/10

Anthropic 首席执行官 Dario Amodei 正在与五角大楼进行紧急磋商，试图挽回上周破裂的 AI 供应协议，此前美国国防部长 Pete Hegseth 已初步将 Anthropic 定性为潜在的供应链风险。若此次补救性谈判失败，Anthropic 将正式被剔除出美军上下游供应链。 这一事件对 Anthropic 构成了重大的商业和战略风险，可能使其失去一个重要政府客户，并为 AI 公司的国家安全审查树立先例。它也凸显了硅谷的伦理承诺与美国政府要求在国防应用中不受限制、合法使用先进 AI 之间日益紧张的关系。 据报道，五角大楼曾提出删除特定协约段落作为妥协，换取 AI 技术可用于其他任何“合法”目的，但遭到 Anthropic 质疑。将一家美国公司定性为供应链风险是前所未有的，这种定性通常只适用于与中国等外国政府有关联的公司。

telegram · zaihuapd · Mar 6, 04:09

**背景**: Anthropic 是一家以开发 Claude 大语言模型而闻名的 AI 安全与研究公司。美国国防部正越来越多地将 AI 整合到其行动中，这导致了与科技公司复杂的采购协议。“供应链风险”定性是一种正式评估，认定某公司的产品或服务对国家安全构成潜在威胁，通常是由于外国所有权、控制权或影响力，并可能导致其被排除在联邦合同之外。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/03/05/technology/anthropic-supply-chain-risk-defense-department.html">Pentagon Officially Notifies Anthropic It Is a ‘ Supply Chain Risk’</a></li>
<li><a href="https://news.northeastern.edu/2026/03/05/anthropic-supply-chain-risk/">What Does It Mean That Anthropic is a ‘Supply Chain’ Risk?</a></li>
<li><a href="https://www.mayerbrown.com/en/insights/publications/2026/03/pentagon-designates-anthropic-a-supply-chain-risk-what-government-contractors-need-to-know">Pentagon Designates Anthropic a Supply Chain Risk — What ...</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Geopolitics`, `#Supply Chain`, `#Anthropic`, `#Defense`

---

<a id="item-9"></a>
## [荷兰暂停《商品可得性法》干预，将安世半导体控制权归还中国母公司闻泰科技](https://t.me/zaihuapd/40069) ⭐️ 8.0/10

荷兰政府于 11 月 19 日宣布，暂停依据《商品可得性法》对中资芯片制造商安世半导体 (Nexperia) 实施的干预令，将控制权归还给其中国母公司闻泰科技。荷兰经济事务大臣卡雷曼斯表示，此举是“善意的表示”。 这是欧洲关键技术出口国一次重大的政策转向，直接影响全球半导体供应链和中美科技竞争。此举标志着荷兰在关键技术领域外资所有权问题上的立场可能出现缓和，可能影响欧盟整体对中国在敏感领域投资的监管态度。 荷兰政府最初的干预发生在 2025 年 10 月，当时以公司治理风险和欧洲经济安全为由，将闻泰科技的股份置于托管之下并剥夺了其 CEO 的控制权，据报道此举是在美国施压后进行的。此次暂停令恢复了运营控制权，但《商品可得性法》的法律框架以及未来可能再次干预的机制依然存在。

telegram · zaihuapd · Mar 6, 08:08

**背景**: 安世半导体 (Nexperia) 是一家总部位于荷兰的主要半导体制造商，专注于分立器件、MOSFET 和逻辑 IC。它被中国的闻泰科技收购，由于闻泰科技部分股权由中国国有资产监督管理机构持有，这一收购引发了地缘政治担忧。荷兰《商品可得性法》(Warenwet) 是一部规范荷兰市场交易产品的框架性法律，荷兰政府于 2025 年援引该法，出于对技术转移和公司治理问题的担忧，对安世半导体的管理进行了干预。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nexperia">Nexperia - Wikipedia</a></li>
<li><a href="https://apnews.com/article/nexperia-wingtech-chips-netherlands-china-f1d3c84065cb61a1d645b64a3a2a68fc">Dutch government intervenes in Chinese-owned semiconductor ...</a></li>
<li><a href="https://business.gov.nl/regulation/commodities-act/">The Dutch Commodities Act (Warenwet) | Business.gov.nl</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#geopolitics`, `#supply-chain`, `#regulation`, `#china-tech`

---

<a id="item-10"></a>
## [研究发现近半数第三方大语言模型中转 API 存在模型不一致问题](https://arxiv.org/abs/2603.01919) ⭐️ 7.0/10

3 月 5 日发布于 arXiv 的一篇研究论文对 17 个被 187 篇学术论文使用的第三方 API 中转服务进行了审计。结果显示，在 24 个测试端点中，45.83%未通过模型身份验证，部分接口在医学和法律等关键领域的测试表现明显低于官方版本，例如在 MedQA 测试中，Gemini-2.5-flash 的准确率从官方的 83.82%降至通过相关中转 API 调用后的平均约 36.95%。 这一发现意义重大，因为它揭示了一个可能损害已发表 AI 研究完整性和可重复性的普遍可靠性问题。依赖这些第三方服务获取模型的研究人员可能在不知情的情况下使用不一致或性能较差的模型，从而导致潜在的无效结论，尤其是在医疗和法律等高风险领域。 该研究通过性能基准测试和模型指纹识别技术来验证这些 API 是否实际调用了它们所声称的模型。审计对象是作为中介、将用户连接到谷歌（Gemini）等提供商官方大语言模型接口的 API，而非官方端点本身。

telegram · zaihuapd · Mar 6, 07:02

**背景**: 第三方 API 中转服务是提供访问 GPT-4 或 Gemini 等大语言模型（LLM）的服务，通常提供简化的定价或访问方式。模型指纹识别是一种通过分析模型输出中的独特模式来识别特定 AI 模型的技术，类似于侦探使用指纹。MedQA 是一个用于评估 AI 模型医学问答能力的基准数据集，包含广泛的医学多项选择题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sandgarden.com/learn/model-fingerprinting">Model Fingerprinting and the Hunt for Stolen AI</a></li>
<li><a href="https://www.vals.ai/benchmarks/medqa">MedQA</a></li>

</ul>
</details>

**标签**: `#AI Research`, `#Model Reliability`, `#API Security`, `#Research Integrity`, `#LLM Evaluation`

---

<a id="item-11"></a>
## [消息称美国海关与边境保护局可利用广告定位数据进行监控](https://www.404media.co/cbp-tapped-into-the-online-advertising-ecosystem-to-track-peoples-movements/) ⭐️ 7.0/10

根据 404 Media 获取的文件，美国海关与边境保护局承认，其在 2019 年至 2021 年的一项试点中使用了“商业可得的营销位置数据”进行监控。其中部分数据来自网络广告实时竞价系统。 这一事件揭示了政府机构如何通过从商业市场购买敏感位置数据，绕过传统的法律保护和监督。它引发了关于隐私、公民自由以及利用原本为广告目的收集的数据进行大规模监控常态化的重大担忧。 据报道，这些数据包括应用与网站在广告竞价或通过软件开发工具包（SDK）时传出的广告标识符、GPS 坐标和 IP 地址等信息。报道还指出，相关联邦机构在该试点期结束后，仍持续采购商业位置追踪工具。

telegram · zaihuapd · Mar 6, 13:48

**背景**: 实时竞价（RTB）是一种程序化广告系统，当用户加载网页或应用时，数字广告展示位会在几毫秒内被拍卖。这个过程通常涉及与多方共享用户数据，如广告标识符和位置信息，以实现广告定向。数据经纪商是从各种来源（包括 RTB 系统和应用 SDK）聚合个人信息并出售给其他企业的公司，从而为精确位置历史等敏感数据创造了一个庞大的市场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Real-time_bidding">Real-time bidding - Wikipedia</a></li>
<li><a href="https://www.eff.org/issues/location-data-brokers">Location Data Brokers | Electronic Frontier Foundation</a></li>

</ul>
</details>

**标签**: `#surveillance`, `#privacy`, `#advertising-technology`, `#government`, `#data-brokers`

---