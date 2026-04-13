---
layout: default
title: "Horizon Summary: 2026-04-13 (ZH)"
date: 2026-04-13
lang: zh
---

> From 18 items, 11 important content pieces were selected

---

1. [所有初等函数可由单一二元运算符构造](#item-1) ⭐️ 9.0/10
2. [Cloudflare 联手 OpenAI 推出 Agent Cloud，支持在边缘网络部署 GPT-5.4 和 Codex 企业级 AI 智能体。](#item-2) ⭐️ 9.0/10
3. [软件工程组织缺乏衡量生产力的经济框架，AI 智能体或将改变开发经济学。](#item-3) ⭐️ 8.0/10
4. [苹果正开发首款 AI 智能眼镜（代号 N50），具备多款镜框风格与独特相机，目标 2026-2027 年发布](#item-4) ⭐️ 8.0/10
5. [欧盟拟将 ChatGPT 列为'超大型在线搜索引擎'，将面临最严数字监管](#item-5) ⭐️ 8.0/10
6. [金山毒霸与 360 安全卫士内核驱动曝高危漏洞](#item-6) ⭐️ 8.0/10
7. [美国出口管制机构人员流失近 20%，英伟达和 AMD 的 AI 芯片出口审批陷入停滞](#item-7) ⭐️ 8.0/10
8. [Bryan Cantrill 认为 LLM 缺乏人类的懒惰性，导致系统臃肿](#item-8) ⭐️ 7.0/10
9. [杜罗夫质疑 WhatsApp 默认加密声明，揭露未加密的云备份](#item-9) ⭐️ 7.0/10
10. [第三方评测称 Claude Opus 4.6 幻觉率大幅上升，排名从第二跌至第十](#item-10) ⭐️ 7.0/10
11. [Cloudflare 数据显示 AI 巨头正打破互联网经济平衡，Anthropic 的“抓取引流比”最为极端](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [所有初等函数可由单一二元运算符构造](https://arxiv.org/abs/2603.21852) ⭐️ 9.0/10

一篇理论论文（arXiv:2603.21852）证明，所有初等函数，如指数、对数和三角函数，都可以从一个名为 EML 的单一二元运算符构造出来。这意味着一个仅配备 EML 运算符和常数'1'的计算系统，原则上可以完成任何科学计算器的全部计算功能。 这一发现对计算数学和函数逼近具有深远意义，可能为复杂函数建模提供一个统一的、极简的基础。它可能彻底改变我们处理数值方法、机器学习（例如，在 EML 树上进行梯度下降）和计算系统设计的方式，将所需的基本运算减少到绝对最低限度。 该运算符名为 EML，其构造依赖于将该单一运算符与自身以及常数 1 进行组合，以生成所有初等函数。这篇论文是理论性的，虽然它证明了通用性，但仅使用 EML 组合来表示常见函数的实际效率和计算复杂度，仍是未来需要探索的领域。

hackernews · pizza · Apr 13, 01:49

**背景**: 在数学中，二元运算将两个元素组合以产生第三个元素，例如加法或乘法。初等函数是标准函数，如多项式、指数、对数和三角函数，它们是科学和工程学的基础。函数逼近是使用更简单的函数（如多项式）来表示更复杂函数的领域，这在数值分析和计算建模中至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Binary_operation">Binary operation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Elementary_function">Elementary function - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Function_approximation">Function approximation - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区反应非常兴奋且参与度高，专家称其为'多年来最重要的发现之一'。讨论强调了在数据建模和波函数建模中的潜在应用，将其与 FRACTRAN 和 Iota 组合子等基础计算概念相类比，并探索了实际实现，例如有用户创建了一个 EML 虚拟机。也有人将论文提出的挑战用作大型语言模型的基准测试。

**标签**: `#theoretical-computer-science`, `#mathematics`, `#function-approximation`, `#computational-complexity`, `#binary-operators`

---

<a id="item-2"></a>
## [Cloudflare 联手 OpenAI 推出 Agent Cloud，支持在边缘网络部署 GPT-5.4 和 Codex 企业级 AI 智能体。](https://openai.com/index/cloudflare-openai-agent-cloud/) ⭐️ 9.0/10

Cloudflare 宣布与 OpenAI 合作，将 OpenAI 的前沿模型（包括 GPT-5.4 和 Codex）接入其 Agent Cloud 平台。数百万企业客户现在可以直接在 Cloudflare 的全球边缘网络上构建并部署 AI 智能体，用于处理客户响应、系统更新等低延迟业务应用。 此次合作标志着 AI 基础设施的重大转变，将先进的 AI 模型推理从集中式数据中心移至网络边缘，能极大降低终端用户的延迟。它为大规模企业级 AI 部署提供了简化方案，OpenAI 的 API 目前每分钟为沃尔玛、埃森哲等客户处理的 Token 数量已超过 1500 亿个，这证明了其处理能力。 该平台基于 Cloudflare Workers AI 运行，这是一个在边缘 GPU 上以无服务器方式运行 AI 模型的平台。包含核心智能体逻辑的 Codex harness 目前已在 Cloudflare Sandboxes（安全的、基于容器的虚拟环境）中上线，并将于近期接入 Workers AI。

telegram · zaihuapd · Apr 13, 13:09

**背景**: Cloudflare Workers AI 是一个平台，允许开发者在 Cloudflare 遍布全球的边缘网络（由靠近终端用户的数据中心组成）上以无服务器方式运行机器学习模型。这种架构旨在通过在地理上更接近数据源的位置进行处理，从而提供低延迟的推理服务。'Codex harness' 指的是支撑 OpenAI 基于 Codex 的智能体的底层系统，它包含了执行任务的核心智能体循环和逻辑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cloudflare.com/developer-platform/products/workers-ai/">Cloudflare Workers AI | Open-source AI inference</a></li>
<li><a href="https://developers.cloudflare.com/workers-ai/">Overview · Cloudflare Workers AI docs</a></li>
<li><a href="https://openai.com/index/unlocking-the-codex-harness/">Unlocking the Codex harness : how we built the App Server | OpenAI</a></li>

</ul>
</details>

**标签**: `#AI-Infrastructure`, `#Edge-Computing`, `#Enterprise-AI`, `#Cloudflare`, `#OpenAI`

---

<a id="item-3"></a>
## [软件工程组织缺乏衡量生产力的经济框架，AI 智能体或将改变开发经济学。](https://www.viktorcessan.com/the-economics-of-software-teams/) ⭐️ 8.0/10

一篇文章分析了大多数软件工程组织如何在缺乏衡量生产力和价值的适当经济框架下运作，使其处于“盲目飞行”状态。文章进一步讨论了 AI 智能体对软件开发基础经济学的潜在影响，表明它们可能彻底改变成本结构和团队构成。 这很重要，因为缺乏可靠的经济衡量标准，工程领导者无法准确优化资源分配、衡量投资回报率或证明投资的合理性，可能导致效率低下和业务价值错位。AI 智能体的兴起可能从根本上重塑软件生产成本和团队经济学，在适应与不适应的组织之间制造竞争鸿沟。 文章认为，对于成熟的、非业务关键的代码，人类对代码的详细熟悉度可能不如以前重要，并且用多个 AI 智能体分析一个混乱的代码库可能比用人力团队维护更便宜。然而，社区评论强烈质疑这一观点，指出 AI 生成的代码尽管能通过表面测试，但可能存在关键的结构性缺陷。

hackernews · kiyanwang · Apr 13, 05:45

**背景**: 软件工程经济学涉及将投资回报率（ROI）、成本效益分析和总拥有成本等经济分析技术应用于软件开发和管理决策。传统上，衡量工程生产力一直具有挑战性，像“代码行数”这样的有缺陷的指标无法捕捉真正的价值或效率。新兴的“智能体经济”描述了一种转变，即 AI 智能体从辅助人类转向自主执行端到端的业务流程，这可能重新定义数字劳动力的经济学。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.computer.org/resources/software-engineering-economics">Software Engineering Economics and Declining Budgets</a></li>
<li><a href="https://www.conductor.com/academy/agent-economy/">The Agent Economy Explained: How AI Agents Are Changing ...</a></li>
<li><a href="https://jellyfish.co/library/engineering-productivity/">How to Measure Engineering Productivity (+ Key Metrics)</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了对于文章关于 AI 智能体的乐观态度存在显著怀疑。一个关键的反驳观点是，软件开发最困难的部分是弄清楚要构建什么，而不是编程本身，而 AI 可能无法解决这一细微差别。其他有直接经验的人引用了失败的 AI 生成项目，警告说智能体产生的代码可能存在标准测试无法发现的隐藏的、灾难性缺陷（例如“用泡沫制成的墙”），这挑战了向问题投入更多智能体是可行解决方案的观点。

**标签**: `#software-engineering`, `#team-productivity`, `#ai-agents`, `#engineering-management`, `#economics`

---

<a id="item-4"></a>
## [苹果正开发首款 AI 智能眼镜（代号 N50），具备多款镜框风格与独特相机，目标 2026-2027 年发布](https://www.bloomberg.com/news/newsletters/2026-04-12/apple-ai-smart-glasses-features-styles-colors-cameras-giannandrea-leaving-mnvtz4yg) ⭐️ 8.0/10

苹果正在开发其首款 AI 驱动的智能眼镜，内部代号为 N50，该产品拥有至少四种不同的镜框风格以及一个独特的垂直定向椭圆形镜头，镜头周围配有灯光。产品计划于 2026 年底或 2027 年初亮相，并于 2027 年正式发布，并将与 iOS 27 中大幅升级的 Siri 深度集成。 这标志着苹果正式战略性地进入 AI 智能眼镜市场，直接与 Meta 的 Ray-Ban Stories 等可穿戴设备竞争，并成为其更广泛的 AI 可穿戴生态系统的一个关键支柱。此类设备的成功，可能通过将 AI 助手与时尚配饰结合，使其具备情境感知能力并无缝融入日常生活，从而重新定义日常的人机交互方式。 这款眼镜将是无显示屏设计，专注于音频和基于摄像头的交互，并且是苹果一系列新 AI 可穿戴设备的一部分，该系列还包括配备摄像头的 AirPods 和一款挂件。据报道，生产计划于 2026 年 12 月开始，该设备将利用计算机视觉技术为 Siri 和 Apple Intelligence 提供情境信息。

telegram · zaihuapd · Apr 13, 01:32

**背景**: 智能眼镜是一类可穿戴计算机，旨在无需手持屏幕即可提供信息和数字交互。Meta（通过 Ray-Ban Stories）和谷歌（历史上通过 Google Glass）等公司已探索这一领域，专注于隐蔽的摄像头、音频和语音助手。'情境感知计算'指的是利用传感器和数据（如位置、摄像头输入或用户活动）来理解用户所处环境，并自动提供相关信息或操作的系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.androidauthority.com/apple-smart-glasses-n50-rumors-3656855/">Apple could outclass Samsung and Google with its smart glasses</a></li>
<li><a href="https://computing.net/news/stocks/apples-ai-smart-glasses-take-shape-with-four-frame-designs-ahead-of-2026-launch/">Apple's AI Smart Glasses Take Shape with Four Frame Designs ...</a></li>
<li><a href="https://technology.amis.nl/amis/google-glass-and-wearable-devices-be-always-context-aware-amis-vision/">Google Glass and Wearable Devices. Always Context Aware - AMIS...</a></li>

</ul>
</details>

**标签**: `#apple`, `#smart-glasses`, `#wearable-tech`, `#artificial-intelligence`, `#computer-vision`

---

<a id="item-5"></a>
## [欧盟拟将 ChatGPT 列为'超大型在线搜索引擎'，将面临最严数字监管](https://www.handelsblatt.com/politik/international/ki-eu-kommission-will-chatgpt-in-zukunft-strenger-regulieren/100215477.html) ⭐️ 8.0/10

欧盟委员会预计将在未来几天内正式宣布，将依据《数字服务法》(DSA) 把 ChatGPT 归类为'超大型在线搜索引擎' (VLOSE)。此举基于数据显示，ChatGPT 在欧洲的月活跃用户已超过 1.2 亿，远超该类别监管所需的 4500 万用户门槛。 此举标志着一个重大的监管转向，将全球最知名的 AI 平台之一置于欧盟最严格的数字治理规则之下。这为生成式 AI 和对话式界面如何在现有平台法律下受到监管开创了先例，可能影响全球类似服务的透明度、算法问责和内容审核实践。 被列为 VLOSE 后，OpenAI 必须遵守 DSA 中最严格的合规要求，包括提高其推荐算法与广告系统的透明度，并采取有效措施防范非法内容及保护用户身心健康。欧盟委员会在分析 ChatGPT 是否符合 DSA 框架下的搜索引擎定义后，预计将很快正式宣布此决定。

telegram · zaihuapd · Apr 13, 08:29

**背景**: 《数字服务法》(DSA) 是欧盟具有里程碑意义的立法，旨在创造一个更安全、更负责任的网络环境。它建立了一个分级监管体系，其中'超大型在线平台'(VLOP)和'超大型在线搜索引擎'(VLOSE)——定义为在欧盟拥有超过 4500 万月活跃用户的服务——面临最严格的义务。这些义务包括风险评估、独立审计、算法透明度以及强有力的内容审核。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Services_Act">Digital Services Act - Wikipedia</a></li>
<li><a href="https://digital-strategy.ec.europa.eu/en/policies/dsa-vlops">DSA: Very large online platforms and search engines</a></li>
<li><a href="https://www.reuters.com/world/openai-faces-tighter-regulation-under-eus-digital-service-act-handelsblatt-says-2026-04-10/">EU weighing tighter regulation for OpenAI under Digital ...</a></li>

</ul>
</details>

**标签**: `#AI Regulation`, `#Digital Services Act`, `#EU Policy`, `#ChatGPT`, `#Platform Governance`

---

<a id="item-6"></a>
## [金山毒霸与 360 安全卫士内核驱动曝高危漏洞](https://x.com/weezerOSINT/status/2043539810833568202?s=20) ⭐️ 8.0/10

安全研究员 Patrick Saif 披露了金山毒霸与 360 安全卫士内核驱动中的高危漏洞。金山毒霸防火墙驱动因 IOCTL 尺寸计算错误引发内核堆溢出，而 360 安全卫士反 Rootkit 驱动存在签名校验绕过和硬编码 AES 密钥问题，两者均允许未经身份验证的攻击者执行任意代码。 此事影响重大，因为这些漏洞影响了中国两款最主流的杀毒软件，能让攻击者从普通用户权限获得内核级访问。这些驱动持有合法的数字签名，极易被用于 BYOVD 攻击，以禁用安全软件并在受感染系统上建立持久性控制。 这两个漏洞已被提交至 LOLDrivers 数据库，但均未获得 CVE 编号，且不在微软 HVCI 屏蔽名单中。利用这些漏洞可实现提权至 SYSTEM、绕过 KASLR、窃取内核凭据以及修改内核回调表以隐藏恶意行为。

telegram · zaihuapd · Apr 13, 13:56

**背景**: 内核驱动在操作系统中以最高权限运行，其中的漏洞危害性极高。IOCTL（输入/输出控制）是用户态应用程序与内核态驱动程序通信的一种机制，处理 IOCTL 请求时的错误可能导致内存损坏。BYOVD（自带漏洞驱动）是一种攻击技术，威胁行为者利用已知漏洞的合法签名驱动来获取内核级访问权限，并常用来禁用安全软件。HVCI（虚拟机监控程序保护的代码完整性）是 Windows 的一项安全功能，它使用屏蔽名单来阻止已知的易受攻击驱动加载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techzone.bitdefender.com/en/tech-explainers/what-is-bring-your-own-vulnerable-driver--byovd-.html">What is Bring Your Own Vulnerable Driver (BYOVD)</a></li>
<li><a href="https://www.elevenforum.com/t/enable-or-disable-microsoft-vulnerable-driver-blocklist-in-windows-11.10031/">Enable or Disable Microsoft Vulnerable Driver Blocklist in Windows 11 | Windows 11 Forum</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerability`, `#kernel-exploitation`, `#antivirus`, `#BYOVD`

---

<a id="item-7"></a>
## [美国出口管制机构人员流失近 20%，英伟达和 AMD 的 AI 芯片出口审批陷入停滞](https://www.tomshardware.com/tech-industry/us-export-control-agency-has-lost-nearly-a-fifth-of-its-licensing-staff) ⭐️ 8.0/10

自 2024 年以来，美国商务部工业和安全局（BIS）已流失 101 名员工，减员比例达 19%，其中负责规则制定和许可审批的人员流失率接近 20%。这导致英伟达和 AMD 等公司 AI 芯片的出口许可平均审批时间从 2023 年的 38 天激增至 2025 年上半年的 76 天，英伟达至今未能向已下单的中国客户交付任何 H200 芯片。 此次人员危机在美国对先进技术的出口管制执行中制造了一个关键瓶颈，直接影响全球 AI 硬件供应链。审批延迟阻碍了中国企业获取 H200 等尖端 AI 芯片，可能影响其 AI 研发进程，同时也给英伟达和 AMD 等美国主要芯片制造商带来了不确定性和财务影响。 除了人员短缺，监管复杂度的提升、内部管理流程的改变，以及商务部副部长杰弗里·凯斯勒坚持亲自审查几乎每一份许可申请，都加剧了审批积压。由于 BIS 尚未发布 2024 和 2025 财年的年度报告，芯片行业目前只能依赖非官方数据来评估申请进度。

telegram · zaihuapd · Apr 13, 15:25

**背景**: 工业和安全局（BIS）是美国商务部下属机构，负责通过对“两用”（兼具民用和军用用途）技术实施出口管制来维护国家安全和外交政策。自 2018 年以来，美国逐步收紧对华先进半导体出口管制，以维持技术领先地位并减缓中国在竞争性 AI 和计算能力方面的发展。英伟达 H200 是一款基于 Hopper 架构的高性能 GPU，旨在为生成式 AI 和高性能计算工作负载提供强大动力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.congress.gov/crs-product/R48642">U.S. Export Controls and China: Advanced Semiconductors</a></li>
<li><a href="https://resources.nvidia.com/en-us-gpu-resources/hpc-datasheet-sc23">NVIDIA H200 GPU Datasheet</a></li>
<li><a href="https://govfacts.org/government/federal/agencies/commerce/a-step-by-step-guide-to-applying-for-a-bis-export-license/">A Step-by-Step Guide to Applying for a BIS Export License</a></li>

</ul>
</details>

**标签**: `#Geopolitics`, `#AI Hardware`, `#Supply Chain`, `#Export Controls`, `#Nvidia`

---

<a id="item-8"></a>
## [Bryan Cantrill 认为 LLM 缺乏人类的懒惰性，导致系统臃肿](https://simonwillison.net/2026/Apr/13/bryan-cantrill/#atom-everything) ⭐️ 7.0/10

软件工程师 Bryan Cantrill 在一篇博客文章中提出，大型语言模型天生缺乏人类的懒惰美德，他将这种懒惰定义为优化未来时间的动力。他认为，由于工作对 LLM 来说没有成本，它会乐于创建层层堆叠的垃圾系统，而缺乏人类那种开发简洁、高效抽象的自然驱动力。 这一观点揭示了 AI 辅助软件开发的一个根本性局限，表明不受约束地使用 LLM 可能导致系统日益庞大和低效，而非变得更好。它迫使开发者和组织审视其 AI 工具中的优化激励（或缺乏激励）问题，可能将关注点从代码行数等虚荣指标转向真正的系统质量和可维护性。 Cantrill 特别警告，LLM 缺乏为任何人的未来时间优化的需求，会诉诸于“反常的虚荣指标”，而牺牲软件中所有重要的东西。他的论点基于一个观察：人类的懒惰是一种美德，它迫使人们创建清晰的抽象，以避免在笨拙的实现上浪费时间。

rss · Simon Willison · Apr 13, 02:44

**背景**: Bryan Cantrill 是一位知名的软件工程师，以其在 Sun Microsystems 公司对 DTrace 的工作以及对系统软件的评论而闻名。软件架构中的“分层蛋糕”或“layer cake”指的是具有多个层级（如表示层、逻辑层和数据层）的设计，如果管理不当，可能会变得臃肿。“虚荣指标”是指那些看起来令人印象深刻（例如代码行数、提交次数）但未必与软件开发中的真正价值或质量相关的度量标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bryan_Cantrill">Bryan Cantrill - Wikipedia</a></li>
<li><a href="https://masterlwa.medium.com/layered-architecture-the-delicious-cake-of-software-architecting-5102e3f80202">Layered Architecture: The Delicious Cake of Software Architecting | by Lakindu Widuranga Alwis | Medium</a></li>
<li><a href="https://www.baytechconsulting.com/blog/future-developer-productivity-metrics-2026">The Future of Developer Productivity: Metrics That Matter</a></li>

</ul>
</details>

**标签**: `#llms`, `#software-engineering`, `#abstraction`, `#optimization`, `#philosophy`

---

<a id="item-9"></a>
## [杜罗夫质疑 WhatsApp 默认加密声明，揭露未加密的云备份](https://t.me/zaihuapd/40826) ⭐️ 7.0/10

Telegram 创始人 Pavel Durov 公开质疑 WhatsApp 宣称的“默认端到端加密”，指出超过 95% 的私人消息以未加密的明文形式存储在苹果或谷歌的云服务器备份中。此外，杜罗夫表示 WhatsApp 会收集用户元数据并与第三方共享，这与 Telegram 声称从未向第三方披露过用户消息数据形成对比。 此事至关重要，因为 WhatsApp 的默认加密声明可能误导其超过 20 亿用户对其通信真实隐私性的认知，营造了一种虚假的安全感。在第三方服务器上以明文形式广泛存储备份的做法，使海量敏感个人数据暴露在云服务提供商、政府或黑客的潜在访问风险之下，从根本上削弱了端到端加密的意义。 一个关键的技术细节是，即使用户开启了加密备份功能，如果聊天对象未进行相同设置，双方的聊天记录仍会以未加密状态存储在各自的云备份中。内容还指出，据报道，苹果和谷歌每年会向第三方披露 WhatsApp 备份数据达数千次。

telegram · zaihuapd · Apr 12, 16:07

**背景**: 端到端加密是一种通信系统，只有参与通信的用户才能阅读消息，防止电信提供商、互联网提供商或服务提供商本身等潜在窃听者获取解密对话所需的加密密钥。元数据是指关于通信的数据（例如，谁与谁通信、时间、时长、地点），即使消息内容被加密，这些数据也能揭示敏感的模式和关系。云备份是应用数据（如聊天记录）的副本，由 iCloud 或 Google Drive 等服务自动存储，以便在不同设备间恢复数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/端到端加密">端到端加密 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.cngold.com.cn/202308107064565348.html">什么是元数据隐私及其为何重要？-新闻资讯-中金网</a></li>

</ul>
</details>

**标签**: `#encryption`, `#privacy`, `#messaging-apps`, `#security`, `#data-protection`

---

<a id="item-10"></a>
## [第三方评测称 Claude Opus 4.6 幻觉率大幅上升，排名从第二跌至第十](https://www.bridgebench.ai/) ⭐️ 7.0/10

AI 评测平台 BridgeMind 发布测试结果称，Claude Opus 4.6 在 BridgeBench 幻觉基准测试中的准确率从上周的 83.3%（排名第 2）下降至 68.3%（排名第 10），降幅约 15 个百分点。平台推测模型推理能力遭到削弱，并建议用户在新版本正式发布前暂缓部署。 这一旗舰 AI 模型的显著性能衰退，对 AI 从业者而言，引发了关于模型稳定性和部署决策可靠性的严重质疑。它凸显了独立、持续的基准测试在追踪模型随时间变化的性能方面所起的关键作用，尤其是在编码等高风险应用中，幻觉可能引入严重错误。 报告指出，Claude Opus 4.6 在该特定基准测试上的幻觉率增加了 98%。值得注意的是，同期 BridgeBench 榜单上的其他头部模型准确率普遍保持在 80% 以上，而 Anthropic 尚未对这些测试结果作出公开回应。

telegram · zaihuapd · Apr 13, 05:00

**背景**: BridgeBench 是由 BridgeMind 构建的一个综合性 AI 编码模型基准测试平台。它从多个类别评估模型，包括幻觉抵抗能力，该指标衡量模型生成错误或虚构信息的倾向。Claude Opus 是 Anthropic 的旗舰大语言模型系列，其 4.6 版本因卓越的推理能力和顶尖的编码能力而被推广。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bridgemind.ai/bridgebench">BridgeBench — Now at bridgebench.ai - bridgemind.ai</a></li>
<li><a href="https://tech.yahoo.com/ai/claude/articles/viral-bridgebench-post-claims-claude-131318087.html">Viral BridgeBench Post Claims Claude Opus 4.6 Was ‘Nerfed ...</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-6">Claude Opus 4.6 \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI Evaluation`, `#Claude`, `#Hallucination`, `#Benchmarking`, `#Model Performance`

---

<a id="item-11"></a>
## [Cloudflare 数据显示 AI 巨头正打破互联网经济平衡，Anthropic 的“抓取引流比”最为极端](https://www.businessinsider.com/ai-bots-strip-mining-web-anthropic-leads-ethical-claude-2026-4) ⭐️ 7.0/10

Cloudflare 最新数据显示，AI 公司在抓取网页内容与回馈流量之间存在严重失衡，其中 Anthropic 的表现最为极端。其“抓取引流比”高达 8800:1，意味着每抓取 8800 次网页仅向原网站发送 1 个点击，这一比例远高于 OpenAI 的 993:1。 这种“只取不予”的行为威胁着互联网传统的“互惠契约”，即爬虫索引内容以换取为发布者带来有价值的流量。由于生成式 AI 聊天机器人倾向于直接提供答案而非引导用户点击源网站，网站主在承担高额爬虫流量成本的同时，却失去了通过引荐流量变现的机会，这可能削弱支撑互联网信息共享的经济引擎。 数据显示，这反映了商业模式的根本差异：Anthropic 的 ClaudeBot 主要作为其 AI 模型的训练数据爬虫运行，这与谷歌等拥有平衡比例的搜索引擎不同。尽管 Anthropic 对统计方法提出过质疑，但行业趋势显示，与传统搜索引擎相比，AI 公司的抓取引流比正在明显恶化。

telegram · zaihuapd · Apr 13, 10:36

**背景**: 网络爬虫是自动程序，用于系统性地浏览互联网以索引内容，传统上由搜索引擎使用。互联网的传统经济模式涉及一种互惠交换：网站允许爬虫索引其内容，作为回报，搜索引擎通过搜索结果将人类访客（流量）送回，发布者可以对此流量进行变现。生成式 AI 公司现在使用类似的爬虫来收集大量网络数据以训练其大语言模型（LLM），但它们的产品（如聊天机器人）旨在直接提供综合答案，减少了用户访问原始源网站的需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.businessinsider.com/anthropic-openai-google-perplexity-microsoft-mistral-crawling-web-referrals-cloudflare-2026-1">Anthropic, OpenAI Crawl the Web Even More, and Give Little ...</a></li>
<li><a href="https://seomator.com/blog/crawl-to-refer-ratio-ai-crawlers-llm-bots">GEO Data Report 2026: Which AI Crawlers & LLM Bots Take the ...</a></li>
<li><a href="https://www.eyerys.com/articles/news/anthropic-has-highest-crawl-refer-ratio-threatens-future-web-says-cloudflare">Anthropic Has The Highest Crawl-To-Refer Ratio, Threatens The ...</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Web Crawling`, `#Internet Economics`, `#Cloudflare`, `#Generative AI`

---