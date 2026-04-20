---
layout: default
title: "Horizon Summary: 2026-04-20 (ZH)"
date: 2026-04-20
lang: zh
---

> From 22 items, 10 important content pieces were selected

---

1. [调查揭露 GitHub 虚假星标市场泛滥，扭曲项目流行度指标。](#item-1) ⭐️ 8.0/10
2. [行业领袖拥抱面向 AI Agent 的'无头'服务，预示 API 优先的架构转变](#item-2) ⭐️ 8.0/10
3. [Vercel 内部系统遭黑客入侵，核心源码及敏感令牌被公开出售](#item-3) ⭐️ 8.0/10
4. [马斯克的 xAI 面临拟议集体诉讼，指控其 Grok AI 将未成年人真实照片生成为 CSAM。](#item-4) ⭐️ 8.0/10
5. [月之暗面发布开源 Kimi K2.6 模型，编码性能达 SOTA 级别](#item-5) ⭐️ 8.0/10
6. [欧盟规定自 2027 年起所有手机和平板电脑必须配备用户可更换电池](#item-6) ⭐️ 7.0/10
7. [蓝色起源成功回收新格伦号火箭，但未能将载荷送入预定轨道](#item-7) ⭐️ 7.0/10
8. [Vercel 确认因第三方 AI 工具漏洞遭黑客攻击，导致员工记录和客户环境变量泄露。](#item-8) ⭐️ 7.0/10
9. [SP 基因家族被确定为肢体再生的潜在主开关，小鼠研究显示部分修复效果](#item-9) ⭐️ 7.0/10
10. [阿里上线 Qwen3.6-Max-Preview 预览版，智能体编程能力大幅提升](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [调查揭露 GitHub 虚假星标市场泛滥，扭曲项目流行度指标。](https://awesomeagents.ai/news/github-fake-stars-investigation/) ⭐️ 8.0/10

近期一项调查系统性地揭露了购买虚假 GitHub 星标的黑市，分析证实，操纵迹象最明显的仓库绝大多数是区块链和加密相关的 AI 项目。该研究还强调了 GitHub 执行的不对称性，即有时会删除仓库，但用于操纵的大部分虚假账户仍然活跃。 这很重要，因为 GitHub 星标被广泛用作项目流行度、质量和社区采用度的代理指标，影响着开发者、投资者甚至风险投资家的决策。这一关键指标的扭曲破坏了开源生态系统的信任，可能导致资金和关注度基于人为夸大的信号而非真实价值进行错误分配。 像 StarScout 这样的研究工具在 2019 年至 2024 年间在 GitHub 上检测到了数百万个疑似虚假星标。一个关键发现是，GitHub 当前的执法行动会删除一些违规仓库，但超过一半的相关虚假账户仍然存在，这保留了重复违规的基础设施，对遏制该市场作用甚微。

hackernews · Liriel · Apr 20, 08:26

**背景**: 在 GitHub 上，“星标”是用户可以点击以收藏或表示对某个仓库赞赏的按钮，类似于“点赞”。随着时间的推移，星标数量已演变为一个被广泛关注的指标，用于衡量项目的流行度、吸引力和社区兴趣。开发者常用此指标来评估采用哪些库或工具，投资者也将其视为项目潜在成功的信号。然而，其简单性使其容易被操纵。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://awesomeagents.ai/news/github-fake-stars-investigation/">Inside GitHub's Fake Star Economy | Awesome Agents</a></li>
<li><a href="https://arxiv.org/abs/2412.13459">[2412.13459] Six Million (Suspected) Fake Stars in GitHub : A Growing...</a></li>
<li><a href="https://www.wired.com/story/github-stars-black-market-coders-cheat/">The GitHub Black Market That Helps Coders Cheat the... | WIRED</a></li>

</ul>
</details>

**社区讨论**: 社区评论对星标的可靠性表示怀疑，一些人质疑风险投资家为何会基于这样的指标做出投资决策。另一些人指出，他们个人更依赖更实质性的信号，如最近的提交活动、问题处理情况和代码质量。一种更广泛的看法认为，这是一个系统性问题，科技领域的所有信号渠道都在变成制成品，这表明问题比 GitHub 星标本身更为深刻。

**标签**: `#github`, `#developer-ecosystem`, `#metrics`, `#software-business`, `#fraud`

---

<a id="item-2"></a>
## [行业领袖拥抱面向 AI Agent 的'无头'服务，预示 API 优先的架构转变](https://simonwillison.net/2026/Apr/19/headless-everything/#atom-everything) ⭐️ 8.0/10

Salesforce 推出了'Headless 360'平台，将其全套服务（Salesforce、Agentforce、Slack）完全通过 API、MCP 工具和 CLI 命令对外暴露，专为 AI Agent 直接交互而设计。此举与分析人士 Matt Webb 的预测一致，即服务将朝着为 AI Agent 交互而非人类 GUI 界面优化的'无头'（headless）趋势发展。 这种向 API 优先、'无头'架构的转变，代表了由个人 AI Agent 兴起驱动的软件消费方式的根本性变革。它可能颠覆传统的按用户计费的 SaaS 定价模式，并成为关键竞争差异点，因为缺乏强大 API 的服务可能会被排除在 AI Agent 的工作流之外。 Salesforce 的实现特别提到了对 Model Context Protocol (MCP)的支持，这是一个在连接 AI Agent 与工具和数据源方面日益流行的标准。分析指出，这种模式对现有的'按人头'计费的 SaaS 定价构成了挑战，因为通过 API 交互的 AI Agent 并不符合传统的用户席位许可模式。

rss · Simon Willison · Apr 19, 21:46

**背景**: '无头架构'（Headless Architecture）将后端服务和数据（'身体'）与前端的展示层（'头'）解耦，使得核心功能可以纯粹通过 API 进行访问。这种方法在内容管理和电子商务中很常见，能够灵活地在不同设备和渠道上交付体验。Model Context Protocol (MCP) 是一个新兴标准，它为 AI Agent 提供了对上下文、数据源和工具的结构化访问，从而增强其能力，而无需为每项服务进行定制化集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://prismic.io/glossary/headless-architecture">What is a Headless Architecture? Definition, Examples, & More</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://www.salesforce.com/news/stories/salesforce-headless-360-announcement/?bc=OTH">Introducing Salesforce Headless 360. No Browser Required.</a></li>

</ul>
</details>

**标签**: `#AI-agents`, `#API-design`, `#software-architecture`, `#future-of-work`, `#SaaS`

---

<a id="item-3"></a>
## [Vercel 内部系统遭黑客入侵，核心源码及敏感令牌被公开出售](https://breachforums.ai/Thread-VERIFIED-Vercel-Database-Access-Key-Source-Code-19-Apr-2026) ⭐️ 8.0/10

云托管平台 Vercel 确认其内部系统遭遇未经授权访问，黑客组织 ShinyHunters 声称已获取其核心源代码及数据库访问权限。该组织已在暗网论坛以 200 万美元的价格挂牌出售包含 API 密钥、NPM 令牌及 GitHub 令牌在内的敏感数据。 此次泄露事件构成了重大的供应链安全风险，因为泄露内容涉及 Next.js 等核心生态的内部部署权限，可能影响数百万开发者和应用程序。敏感令牌的暴露可能使攻击者能够入侵托管在 Vercel 上的下游项目和用户数据。 Vercel 官方已介入调查并通知执法部门，初步确认部分客户受到影响，并建议所有用户立即审查并重置敏感环境变量。此次入侵与以实施高知名度数据泄露和勒索而闻名的 ShinyHunters 组织有关。

telegram · zaihuapd · Apr 19, 16:33

**背景**: Vercel 是一个流行的前端框架云平台，以托管和部署 Next.js 应用程序而闻名。NPM 令牌是用于在 npm 软件包注册表上发布或管理软件包的访问凭证，其泄露可能导致供应链攻击，即恶意代码被注入广泛使用的软件库中。ShinyHunters 是一个臭名昭著的黑客和勒索组织，据信成立于 2019 年左右，并参与了众多重大的数据泄露事件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ShinyHunters">ShinyHunters - Wikipedia</a></li>
<li><a href="https://thecyberedition.com/npm-supply-chain-risks/">npm Tokens Enable Supply Attacks - Cyber Edition</a></li>

</ul>
</details>

**标签**: `#security`, `#vercel`, `#data-breach`, `#supply-chain-security`, `#nextjs`

---

<a id="item-4"></a>
## [马斯克的 xAI 面临拟议集体诉讼，指控其 Grok AI 将未成年人真实照片生成为 CSAM。](https://t.me/zaihuapd/40968) ⭐️ 8.0/10

3 月 16 日，三名来自美国田纳西州的未成年女孩及其监护人在联邦地区法院提起拟议集体诉讼，指控埃隆·马斯克的 xAI 旗下 Grok AI 将她们的真实照片生成了儿童性虐待材料（CSAM）。原告称公司“有意设计”相关功能以牟利，并要求法院发布禁令并索赔，包括惩罚性赔偿。 这起诉讼对生成式 AI 公司构成了重大的法律和伦理挑战，直接检验了它们对有害输出的责任以及内容审核保障措施的充分性。其结果可能为如何追究 AI 开发者责任、防止生成非法和虐待性内容（尤其是涉及儿童安全的内容）开创先例。 据报道，此案是由一名匿名 Discord 用户提示 AI 并随后联系受害者后引发的，最终导致执法部门介入。与此形成鲜明对比的是，埃隆·马斯克在今年 1 月曾表示，未发现 Grok 生成任何未成年人裸露图像。

telegram · zaihuapd · Apr 20, 15:04

**背景**: Grok 是由埃隆·马斯克的公司 xAI 开发的生成式 AI 聊天机器人，以其与 X 平台的整合以及常以“言论自由”承诺为特征的公开立场而闻名。儿童性虐待材料（CSAM）是一个法律术语，指描绘对未成年人进行性虐待的内容；根据美国联邦法律，其制作、持有或传播将面临严厉的刑事处罚。xAI 有一份《可接受使用政策》，禁止非法或有害行为，包括生成 CSAM，但诉讼指控其存在为牟利而故意设计的功能缺陷。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://legalclarity.org/csam-meaning-what-is-child-sexual-abuse-material/">CSAM Meaning: Federal Definition and Criminal Penalties</a></li>
<li><a href="https://factually.co/fact-checks/technology/grok-xai-official-public-moderation-appeals-policies-where-published-cd165b">What are Grok/xAI’s official public moderation and app...</a></li>
<li><a href="https://x.ai/legal/acceptable-use-policy">Acceptable Use Policy - xAI</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Legal`, `#xAI`, `#Content Moderation`, `#Child Safety`

---

<a id="item-5"></a>
## [月之暗面发布开源 Kimi K2.6 模型，编码性能达 SOTA 级别](https://x.com/Kimi_Moonshot/status/2046249571882500354?s=20) ⭐️ 8.0/10

月之暗面（Moonshot AI）正式发布了 Kimi K2.6 模型，该模型在 SWE-Bench Pro 等多项基准测试中取得了 SOTA 成绩。该模型显著提升了长程执行与多智能体协作能力，支持超过 12 小时的连续执行和 4000 次以上的工具调用。 此次发布意义重大，因为它为复杂的软件工程任务和自主 AI 智能体系统提供了一个强大的开源基础。在极具挑战性的 SWE-Bench Pro 基准测试中达到 SOTA 水平，表明该模型有潜力处理现实世界中多步骤的编码问题，这可能会加速自动化软件维护和多智能体工作流等领域的发展。 该模型支持多达 300 个并行子智能体协作，单次运行步数提升至 4000 步，可实现全天候自主运行。模型已在 Kimi 官网及 API 平台上线，其模型权重与代码也已同步开源。

telegram · zaihuapd · Apr 20, 15:40

**背景**: SWE-Bench Pro 是一个高级基准测试，旨在评估语言模型在需要扩展推理和多步骤问题解决的复杂、现实世界软件工程任务上的表现，它超越了简单的代码生成。模型的上下文窗口决定了其一次性能处理的最大信息量（包括提示词和输出），这对于冗长复杂的任务至关重要；长上下文能力与检索增强生成（RAG）是互补的技术。多智能体协作指的是多个 AI 智能体协同工作以解决问题的系统，这代表了从单一 LLM 向能够处理更复杂工作流的分布式、协调式 AI 系统的演进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://llm-stats.com/benchmarks/swe-bench-pro">SWE-Bench Pro Leaderboard - llm-stats.com</a></li>
<li><a href="https://datanorth.ai/blog/context-length">Context Length in LLMs: What Is It and Why It Is Important?</a></li>
<li><a href="https://www.ibm.com/think/topics/multi-agent-collaboration">What is multi-agent collaboration? - IBM</a></li>

</ul>
</details>

**标签**: `#AI-ML`, `#Large-Language-Models`, `#Code-Generation`, `#Open-Source`, `#AI-Agents`

---

<a id="item-6"></a>
## [欧盟规定自 2027 年起所有手机和平板电脑必须配备用户可更换电池](https://www.theolivepress.es/spain-news/2026/04/20/eu-to-force-replaceable-batteries-in-phones-and-tablets-from-2027/) ⭐️ 7.0/10

欧盟的《电池法规》(EU) 2023/1542 规定，从 2027 年起，在欧盟销售的所有手机和平板电脑中的便携式电池必须是用户可更换的。这意味着制造商必须设计出能让消费者无需专业工具即可自行拆卸和更换电池的设备。 这项法规代表了消费电子产品设计的一次重大转变，旨在延长设备寿命并显著减少电子垃圾。它将迫使全球制造商为欧盟市场重新设计产品，可能影响全球标准，并赋予消费者更大的维修权。 该法规包含一个值得注意的豁免条款：能够承受 1000 次充电循环且容量保持在 80%以上的电池不受可更换性要求的约束。这个技术漏洞意味着，像近期 iPhone 这样拥有异常耐用电池的高端设备可能获得豁免，而低成本手机将最受设计变更的影响。

hackernews · ramonga · Apr 20, 13:41

**背景**: 欧盟《电池法规》(EU) 2023/1542 是欧洲绿色协议的一部分，该协议是一项旨在使欧盟经济可持续发展的更广泛倡议。近年来，大多数智能手机制造商为了追求更纤薄的设计和防水性能，都转向了密封、不可拆卸的电池，这使得用户自行更换变得困难。该法规旨在对抗计划性淘汰以及废弃设备产生的日益严重的电子垃圾问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.intertek.com/blog/2025/06-27-2027-reqs-for-removability-and-replaceability-of-batteries-in-electrical-products/">Navigating 2027 requirements for removability and replaceability of batteries in electrical products</a></li>
<li><a href="https://www.compliancegate.com/batteries-regulation-european-union/">EU Batteries Regulation: An Essential Guide</a></li>
<li><a href="https://www.msn.com/en-in/money/news/smartphones-may-get-bigger-user-replaceable-batteries-by-2027-here-is-why/ar-AA21hlCE">Smartphones may get bigger, user - replaceable batteries by 2027...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了不同的观点。一些人质疑其必要性，认为目前的电池已经可以由专业人员更换，并且软件更新比硬件更能导致设备淘汰。另一些人则认为这是积极的一步，但批评 1000 次循环的豁免条款是给高端品牌留了后门。一些评论还延伸了论点，呼吁为电动汽车制定类似的模块化、可升级的电池标准，以最大限度地实现资源再利用。

**标签**: `#regulation`, `#sustainability`, `#consumer-rights`, `#hardware-design`, `#e-waste`

---

<a id="item-7"></a>
## [蓝色起源成功回收新格伦号火箭，但未能将载荷送入预定轨道](https://www.theverge.com/science/914729/blue-origin-successfully-reused-its-new-glenn-rocket) ⭐️ 7.0/10

蓝色起源（Blue Origin）的新格伦号（New Glenn）火箭在其第二次发射任务中，首次成功回收并重复使用了一级助推器，但由于火箭二级推进问题，未能将 AST SpaceMobile 公司的 BlueBird 7 卫星部署到预定轨道。 此次事件标志着蓝色起源在可重复使用重型运载火箭领域取得了重要里程碑，这对于降低太空进入成本至关重要。然而，载荷部署失败凸显了持续存在的技术挑战，特别是二级火箭的可靠性问题，即使一级火箭成功回收，这些问题也可能导致任务失败。 回收的一级助推器成功降落在着陆平台上，蓝色起源此前已翻新了其热防护系统以更好地承受再入热量。AST SpaceMobile 的 BlueBird 7 卫星被送入低于预期的轨道，导致其无法运行并将进行脱轨处理。

telegram · zaihuapd · Apr 20, 01:31

**背景**: 蓝色起源（Blue Origin）是由杰夫·贝索斯创立的美国私营航空航天公司。其新格伦号（New Glenn）火箭是一种用于轨道任务的重型、部分可重复使用运载火箭，其一级助推器设计可飞行至少 25 次。本次任务旨在为 AST SpaceMobile 公司发射卫星，该公司正在建设一个旨在直接连接标准移动设备的太空蜂窝宽带网络。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.blueorigin.com/new-glenn">New Glenn | Blue Origin</a></li>
<li><a href="https://en.wikipedia.org/wiki/AST_SpaceMobile">AST SpaceMobile - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blue_Origin">Blue Origin - Wikipedia</a></li>

</ul>
</details>

**标签**: `#spaceflight`, `#rocket-technology`, `#blue-origin`, `#satellite`, `#aerospace`

---

<a id="item-8"></a>
## [Vercel 确认因第三方 AI 工具漏洞遭黑客攻击，导致员工记录和客户环境变量泄露。](http://context.ai/) ⭐️ 7.0/10

Vercel 确认发生数据泄露，攻击者利用第三方 AI 工具 Context.ai 的 Google Workspace 授权漏洞，非法访问了其内部系统。此次泄露暴露了 580 条员工记录和部分未加密的客户环境变量，攻击者索要了 200 万美元赎金。 该事件凸显了在云开发生态系统中，第三方集成（尤其是需要深度系统访问权限的 AI 工具）所带来的重大安全风险。它强调了围绕环境变量等敏感数据采取强健安全实践的极端重要性，因为这些变量控制着对应用程序密钥和基础设施的访问。 Vercel 的核心服务及 Next.js 等开源项目未受影响。该公司已敦促用户审查并重置其环境变量，并对非敏感变量实施了加密管理。据报道，此次泄露与通过 Context.ai 平台被入侵的 Vercel 员工账户有关。

telegram · zaihuapd · Apr 20, 02:17

**背景**: Vercel 是一个流行的前端框架云平台，以托管 Next.js 应用程序而闻名。环境变量是存储在应用程序代码之外的配置值，通常用于保存 API 密钥和数据库密码等敏感数据。Context.ai 是一个在企业系统内部署 AI 代理以执行工作流并从用户修正中学习的平台。Google Workspace 授权涉及通过访问令牌授予应用程序对特定资源的访问权限，此过程中的漏洞可能导致账户被接管。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/04/vercel-breach-tied-to-context-ai-hack.html">Vercel Breach Tied to Context AI Hack Exposes Limited ...</a></li>
<li><a href="https://context.ai/security-update">Security Update — Context</a></li>
<li><a href="https://phemex.com/news/article/vercel-employee-implicated-in-contextai-data-breach-74456">Vercel Employee Linked to Context.ai Data Breach - Phemex</a></li>

</ul>
</details>

**标签**: `#security`, `#data-breach`, `#vercel`, `#ai-tools`, `#cloud-platform`

---

<a id="item-9"></a>
## [SP 基因家族被确定为肢体再生的潜在主开关，小鼠研究显示部分修复效果](https://neurosciencenews.com/sp-gene-limb-regeneration-30553/) ⭐️ 7.0/10

一项发表在《美国国家科学院院刊》（PNAS）上的跨物种研究发现，SP 基因家族（特别是 SP6 和 SP8）可能是蝾螈、斑马鱼和小鼠肢体再生的共同调控开关。研究人员利用斑马鱼来源的再生增强子，通过病毒载体递送信号蛋白 FGF8，部分恢复了小鼠的指尖再生能力。 这一发现为激活哺乳动物体内潜在的再生程序提供了一条具体的机制通路，使研究从观察生物学转向了靶向干预。虽然距离人体临床应用还很遥远，但它代表了一个重要的原理验证，可能为未来的组织修复和肢体再生疗法提供信息。 目前的实验验证仅限于小鼠指尖再生，而非完整的肢体再生。该研究使用了斑马鱼来源的组织再生增强子元件（TREE）来递送 FGF8，FGF8 是一种在发育过程中参与细胞增殖和分化的分泌性信号分子。

telegram · zaihuapd · Apr 20, 03:02

**背景**: 像蝾螈和斑马鱼这样的动物拥有显著的再生能力，能够在受伤后重新长出完整的肢体或器官，而像小鼠和人类这样的哺乳动物再生能力非常有限。SP 基因家族，包括 SP8，是已知在墨西哥钝口螈等物种中调节肢体发育和再生的转录因子。成纤维细胞生长因子 8（FGF8）是一种参与胚胎模式形成和器官发生的关键信号蛋白。再生增强子是响应损伤而激活基因表达程序的特定 DNA 序列。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://phys.org/news/2026-04-regrowing-human-limbs-salamander-gene.html">For regrowing human limbs, this salamander gene could hold the key</a></li>
<li><a href="https://pubmed.ncbi.nlm.nih.gov/36495292/">leptin b and its regeneration enhancer illustrate the regenerative ...</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC12197990/">Fibroblast growth factor 8: Multifaceted role in development ...</a></li>

</ul>
</details>

**标签**: `#regenerative-biology`, `#genetics`, `#biotechnology`, `#regenerative-medicine`, `#developmental-biology`

---

<a id="item-10"></a>
## [阿里上线 Qwen3.6-Max-Preview 预览版，智能体编程能力大幅提升](https://mp.weixin.qq.com/s/DKxrFnBwisNjjOnFQRqsqA) ⭐️ 7.0/10

阿里巴巴发布了其旗舰模型 Qwen3.6-Max 的预览版，核心聚焦于智能体编程与世界知识能力的迭代。该模型在 SciCode 与 SkillsBench 基准上分别实现了 10.8 和 9.9 分的分值增长，并在包括 SWE-bench Pro 在内的六项编程评测中位居首位。 此次发布表明大型语言模型在执行复杂、多步骤软件工程任务方面的自主能力取得了显著进步，这对于开发实用的 AI 智能体至关重要。作为主要 AI 参与者，阿里巴巴在智能体编程方面的进展直接与 OpenAI 和 Anthropic 的产品竞争，推动整个行业向更强大、更自主的编程助手发展。 该模型在衡量世界知识与指令遵循的 QwenChineseBench 基准上评分也提升了 5.3 分。目前该模型已接入 Qwen Studio 及阿里云百炼 API，支持保留多轮对话中思考内容的'preserve_thinking'功能，并全面兼容 OpenAI 与 Anthropic 的规范接口。

telegram · zaihuapd · Apr 20, 09:15

**背景**: Qwen3.6 是阿里巴巴通义千问模型家族的最新成员，基于 Qwen3.5 构建，专注于为开发者提供稳定且实用的体验。SWE-bench Pro 是一个高级基准测试，用于评估语言模型在需要扩展推理和多步骤问题解决的复杂、真实世界软件工程任务上的表现。'preserve_thinking'（保留思考）功能是一种能跨越多轮对话保持模型内部推理链的特性，这对于涉及规划和工具使用的智能体工作流程至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/QwenLM/Qwen3.6">GitHub - QwenLM/Qwen3.6: Qwen3.6 is the large language model ...</a></li>
<li><a href="https://llm-stats.com/benchmarks/swe-bench-pro">SWE-Bench Pro Leaderboard</a></li>
<li><a href="https://www.alibabacloud.com/blog/qwen3-6-plus-towards-real-world-agents_603005">Qwen3.6-Plus: Towards Real World Agents - Alibaba Cloud Community</a></li>

</ul>
</details>

**标签**: `#AI Models`, `#Large Language Models`, `#Programming Agents`, `#Alibaba`, `#Benchmarks`

---