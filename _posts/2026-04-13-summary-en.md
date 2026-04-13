---
layout: default
title: "Horizon Summary: 2026-04-13 (EN)"
date: 2026-04-13
lang: en
---

> From 18 items, 11 important content pieces were selected

---

1. [All Elementary Functions Constructed from a Single Binary Operator](#item-1) ⭐️ 9.0/10
2. [Cloudflare and OpenAI launch Agent Cloud, enabling enterprise deployment of GPT-5.4 and Codex on the edge.](#item-2) ⭐️ 9.0/10
3. [Software engineering organizations lack economic frameworks for measuring productivity, with AI agents poised to change development economics.](#item-3) ⭐️ 8.0/10
4. [Apple Developing First AI Smart Glasses (N50) with Multiple Frame Styles and Unique Camera, Targeting 2026-2027 Release](#item-4) ⭐️ 8.0/10
5. [EU Plans to Classify ChatGPT as a 'Very Large Online Search Engine' Under Strict Digital Rules](#item-5) ⭐️ 8.0/10
6. [High-risk kernel driver vulnerabilities disclosed in Kingsoft Antivirus and 360 Safeguard](#item-6) ⭐️ 8.0/10
7. [U.S. Export Control Agency Loses 20% of Staff, Stalling AI Chip Approvals for Nvidia and AMD](#item-7) ⭐️ 8.0/10
8. [Bryan Cantrill argues LLMs lack human laziness, leading to bloated systems](#item-8) ⭐️ 7.0/10
9. [Durov Challenges WhatsApp's Default Encryption Claims, Reveals Unencrypted Cloud Backups](#item-9) ⭐️ 7.0/10
10. [Third-party benchmark reports Claude Opus 4.6 hallucination rate surged, ranking drops from 2nd to 10th](#item-10) ⭐️ 7.0/10
11. [Cloudflare Data Shows AI Giants Disrupting Web's Economic Balance, Anthropic's 'Crawl-to-Refer' Ratio Most Extreme](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [All Elementary Functions Constructed from a Single Binary Operator](https://arxiv.org/abs/2603.21852) ⭐️ 9.0/10

A theoretical paper (arXiv:2603.21852) demonstrates that all elementary functions, such as exponentials, logarithms, and trigonometric functions, can be constructed from a single binary operator called EML. This means a computational system equipped only with the EML operator and the constant '1' can, in principle, compute anything a full scientific calculator can. This discovery has profound implications for computational mathematics and function approximation, potentially offering a unified, minimalistic foundation for modeling complex functions. It could revolutionize how we approach numerical methods, machine learning (e.g., gradient descent on EML trees), and the design of computational systems by reducing the required primitive operations to an absolute minimum. The operator is named EML, and the construction relies on composing this single operator with itself and the constant 1 to generate all elementary functions. The paper is theoretical, and while it proves universality, the practical efficiency and computational complexity of representing common functions using only EML compositions remain areas for future exploration.

hackernews · pizza · Apr 13, 01:49

**Background**: In mathematics, a binary operation combines two elements to produce a third, such as addition or multiplication. Elementary functions are standard functions like polynomials, exponentials, logarithms, and trigonometric functions, which are foundational in science and engineering. Function approximation is the field of using simpler functions (like polynomials) to represent more complex ones, which is crucial in numerical analysis and computational modeling.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Binary_operation">Binary operation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Elementary_function">Elementary function - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Function_approximation">Function approximation - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community reaction is highly excited and engaged, with experts calling it 'one of the most significant discoveries in years.' Discussions highlight potential applications in modeling data and wave functions, draw parallels to foundational computational concepts like FRACTRAN and the Iota combinator, and explore practical implementations, such as a user creating an EML virtual machine. Some also used the paper's challenge as a benchmark for large language models.

**Tags**: `#theoretical-computer-science`, `#mathematics`, `#function-approximation`, `#computational-complexity`, `#binary-operators`

---

<a id="item-2"></a>
## [Cloudflare and OpenAI launch Agent Cloud, enabling enterprise deployment of GPT-5.4 and Codex on the edge.](https://openai.com/index/cloudflare-openai-agent-cloud/) ⭐️ 9.0/10

Cloudflare has partnered with OpenAI to integrate OpenAI's advanced models, including GPT-5.4 and Codex, into its Agent Cloud platform. This enables over one million enterprise customers to build and deploy AI agents directly on Cloudflare's global edge network for low-latency business applications like automated customer responses and report generation. This partnership represents a major infrastructure shift, moving advanced AI model inference from centralized data centers to the network edge, which can drastically reduce latency for end-users. It simplifies enterprise AI deployment at massive scale, as evidenced by the existing processing of over 150 billion tokens per minute through OpenAI's API for clients like Walmart and Accenture. The platform runs on Cloudflare Workers AI, a serverless platform for running AI models on GPUs at the edge. The Codex harness, which contains the core agent logic, is now available within Cloudflare Sandboxes—secure, container-based virtual environments—and will soon be integrated into Workers AI.

telegram · zaihuapd · Apr 13, 13:09

**Background**: Cloudflare Workers AI is a platform that allows developers to run machine learning models in a serverless manner on Cloudflare's global edge network, which consists of data centers close to end-users. This architecture is designed to provide low-latency inference by processing data geographically closer to its source. The 'Codex harness' refers to the underlying system that powers OpenAI's Codex-based agents, containing the core agent loop and logic for executing tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cloudflare.com/developer-platform/products/workers-ai/">Cloudflare Workers AI | Open-source AI inference</a></li>
<li><a href="https://developers.cloudflare.com/workers-ai/">Overview · Cloudflare Workers AI docs</a></li>
<li><a href="https://openai.com/index/unlocking-the-codex-harness/">Unlocking the Codex harness : how we built the App Server | OpenAI</a></li>

</ul>
</details>

**Tags**: `#AI-Infrastructure`, `#Edge-Computing`, `#Enterprise-AI`, `#Cloudflare`, `#OpenAI`

---

<a id="item-3"></a>
## [Software engineering organizations lack economic frameworks for measuring productivity, with AI agents poised to change development economics.](https://www.viktorcessan.com/the-economics-of-software-teams/) ⭐️ 8.0/10

An article analyzes how most software engineering organizations operate without proper economic frameworks to measure productivity and value, leaving them "flying blind." It further discusses the potential impact of AI agents on the fundamental economics of software development, suggesting they could drastically alter cost structures and team composition. This matters because without sound economic measurement, engineering leaders cannot accurately optimize resource allocation, measure ROI, or justify investments, potentially leading to inefficiency and misaligned business value. The rise of AI agents could fundamentally reshape software production costs and team economics, creating a competitive divide between organizations that adapt and those that do not. The article argues that for established, non-business-critical code, detailed human familiarity may matter less than before, and a messy codebase could be cheaper to analyze with multiple AI agents than to maintain with a human team. However, community comments strongly challenge this view, pointing out that AI-generated code can have critical structural flaws despite passing superficial tests.

hackernews · kiyanwang · Apr 13, 05:45

**Background**: Software engineering economics involves applying economic analysis techniques—such as return on investment (ROI), cost-benefit analysis, and total cost of ownership—to software development and management decisions. Traditionally, measuring engineering productivity has been challenging, with flawed metrics like "lines of code" failing to capture true value or efficiency. The emerging "agent economy" describes a shift where AI agents move from assisting humans to autonomously executing end-to-end business workflows, which could redefine the economics of digital labor.

<details><summary>References</summary>
<ul>
<li><a href="https://www.computer.org/resources/software-engineering-economics">Software Engineering Economics and Declining Budgets</a></li>
<li><a href="https://www.conductor.com/academy/agent-economy/">The Agent Economy Explained: How AI Agents Are Changing ...</a></li>
<li><a href="https://jellyfish.co/library/engineering-productivity/">How to Measure Engineering Productivity (+ Key Metrics)</a></li>

</ul>
</details>

**Discussion**: The community discussion reveals significant skepticism toward the article's optimism about AI agents. A key counterargument is that the hardest part of software development is figuring out what to build, not the programming itself, a nuance AI may not address. Others with direct experience cite failed AI-generated projects, warning that agent-produced code can have hidden, catastrophic flaws (like "walls made of foam") that aren't caught by standard tests, challenging the notion that throwing more agents at a problem is a viable solution.

**Tags**: `#software-engineering`, `#team-productivity`, `#ai-agents`, `#engineering-management`, `#economics`

---

<a id="item-4"></a>
## [Apple Developing First AI Smart Glasses (N50) with Multiple Frame Styles and Unique Camera, Targeting 2026-2027 Release](https://www.bloomberg.com/news/newsletters/2026-04-12/apple-ai-smart-glasses-features-styles-colors-cameras-giannandrea-leaving-mnvtz4yg) ⭐️ 8.0/10

Apple is developing its first AI-powered smart glasses, internally codenamed N50, with at least four distinct frame styles and a unique vertically oriented oval camera lens surrounded by lights. The product is planned for a late 2026 or early 2027 unveiling, with a full release in 2027, and will integrate with a significantly upgraded Siri in iOS 27. This marks Apple's strategic entry into the AI-powered smart glasses market, directly competing with Meta's Ray-Ban Stories and other wearables, and represents a key pillar of its broader wearable AI ecosystem. The success of such a device could redefine everyday human-computer interaction by making AI assistance context-aware and seamlessly integrated into daily life through a fashionable accessory. The glasses will be display-less, focusing on audio and camera-based interactions, and are part of a suite of new AI wearables that includes camera-equipped AirPods and a pendant. Production is reportedly scheduled to begin in December 2026, and the device will leverage computer vision to provide context for Siri and Apple Intelligence.

telegram · zaihuapd · Apr 13, 01:32

**Background**: Smart glasses are a category of wearable computers that aim to provide information and digital interaction without requiring a handheld screen. Companies like Meta (with Ray-Ban Stories) and Google (with Glass, historically) have explored this space, focusing on discreet cameras, audio, and voice assistants. 'Context-aware computing' refers to systems that use sensors and data (like location, camera input, or user activity) to understand a user's situation and provide relevant information or actions automatically.

<details><summary>References</summary>
<ul>
<li><a href="https://www.androidauthority.com/apple-smart-glasses-n50-rumors-3656855/">Apple could outclass Samsung and Google with its smart glasses</a></li>
<li><a href="https://computing.net/news/stocks/apples-ai-smart-glasses-take-shape-with-four-frame-designs-ahead-of-2026-launch/">Apple's AI Smart Glasses Take Shape with Four Frame Designs ...</a></li>
<li><a href="https://technology.amis.nl/amis/google-glass-and-wearable-devices-be-always-context-aware-amis-vision/">Google Glass and Wearable Devices. Always Context Aware - AMIS...</a></li>

</ul>
</details>

**Tags**: `#apple`, `#smart-glasses`, `#wearable-tech`, `#artificial-intelligence`, `#computer-vision`

---

<a id="item-5"></a>
## [EU Plans to Classify ChatGPT as a 'Very Large Online Search Engine' Under Strict Digital Rules](https://www.handelsblatt.com/politik/international/ki-eu-kommission-will-chatgpt-in-zukunft-strenger-regulieren/100215477.html) ⭐️ 8.0/10

The European Commission is expected to formally announce within days that it will classify ChatGPT as a 'Very Large Online Search Engine' (VLOSE) under the Digital Services Act (DSA). This classification is based on data showing ChatGPT has over 120 million monthly active users in Europe, far exceeding the 45 million user threshold for VLOSE designation. This represents a significant regulatory shift, subjecting one of the world's most prominent AI platforms to the EU's strictest digital governance rules. It sets a precedent for how generative AI and conversational interfaces may be regulated under existing platform laws, potentially affecting transparency, algorithmic accountability, and content moderation practices for similar services globally. As a VLOSE, OpenAI will be required to comply with the most stringent tier of DSA obligations, including enhancing transparency of its recommendation algorithms and advertising systems, and implementing effective measures to prevent illegal content and protect users' physical and mental well-being. The formal announcement is anticipated imminently, following the Commission's analysis of whether ChatGPT qualifies as a search engine under the DSA framework.

telegram · zaihuapd · Apr 13, 08:29

**Background**: The Digital Services Act (DSA) is the EU's landmark legislation designed to create a safer and more accountable online environment. It establishes a tiered regulatory system where 'Very Large Online Platforms' (VLOPs) and 'Very Large Online Search Engines' (VLOSEs) — defined as those with over 45 million monthly active users in the EU — face the most stringent obligations. These obligations include risk assessments, independent auditing, transparency around algorithms, and robust content moderation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Services_Act">Digital Services Act - Wikipedia</a></li>
<li><a href="https://digital-strategy.ec.europa.eu/en/policies/dsa-vlops">DSA: Very large online platforms and search engines</a></li>
<li><a href="https://www.reuters.com/world/openai-faces-tighter-regulation-under-eus-digital-service-act-handelsblatt-says-2026-04-10/">EU weighing tighter regulation for OpenAI under Digital ...</a></li>

</ul>
</details>

**Tags**: `#AI Regulation`, `#Digital Services Act`, `#EU Policy`, `#ChatGPT`, `#Platform Governance`

---

<a id="item-6"></a>
## [High-risk kernel driver vulnerabilities disclosed in Kingsoft Antivirus and 360 Safeguard](https://x.com/weezerOSINT/status/2043539810833568202?s=20) ⭐️ 8.0/10

Security researcher Patrick Saif disclosed high-risk vulnerabilities in the kernel drivers of Kingsoft Antivirus and 360 Safeguard. The Kingsoft firewall driver has a kernel heap overflow due to an IOCTL size calculation error, while the 360 anti-rootkit driver has a flawed signature check and a hardcoded AES key, both allowing unauthenticated attackers to execute arbitrary code. This matters because these vulnerabilities affect two of the most widely used antivirus products in China, granting attackers kernel-level access from a standard user account. The drivers hold legitimate digital signatures, making them prime targets for BYOVD attacks to disable security software and establish persistence on compromised systems. Both vulnerabilities have been added to the LOLDrivers database but lack CVE IDs and are not on Microsoft's HVCI blocklist. Exploitation can lead to privilege escalation to SYSTEM, bypassing KASLR, stealing kernel credentials, and modifying kernel callback tables to hide malicious activity.

telegram · zaihuapd · Apr 13, 13:56

**Background**: Kernel drivers run with the highest privileges in an operating system, and vulnerabilities in them are severe. IOCTL (Input/Output Control) is a mechanism for user-mode applications to communicate with kernel-mode drivers; errors in handling IOCTL requests can lead to memory corruption. BYOVD (Bring Your Own Vulnerable Driver) is an attack technique where threat actors exploit legitimate, signed drivers with known vulnerabilities to gain kernel-level access and often disable security software. HVCI (Hypervisor-protected Code Integrity) is a Windows security feature that uses a blocklist to prevent known vulnerable drivers from loading.

<details><summary>References</summary>
<ul>
<li><a href="https://techzone.bitdefender.com/en/tech-explainers/what-is-bring-your-own-vulnerable-driver--byovd-.html">What is Bring Your Own Vulnerable Driver (BYOVD)</a></li>
<li><a href="https://www.elevenforum.com/t/enable-or-disable-microsoft-vulnerable-driver-blocklist-in-windows-11.10031/">Enable or Disable Microsoft Vulnerable Driver Blocklist in Windows 11 | Windows 11 Forum</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#vulnerability`, `#kernel-exploitation`, `#antivirus`, `#BYOVD`

---

<a id="item-7"></a>
## [U.S. Export Control Agency Loses 20% of Staff, Stalling AI Chip Approvals for Nvidia and AMD](https://www.tomshardware.com/tech-industry/us-export-control-agency-has-lost-nearly-a-fifth-of-its-licensing-staff) ⭐️ 8.0/10

The U.S. Bureau of Industry and Security (BIS) has lost 101 employees since 2024, a 19% reduction in staff, with nearly 20% of its rule-making and licensing personnel leaving. This has caused the average processing time for export licenses for AI chips from companies like Nvidia and AMD to double from 38 days in 2023 to 76 days in the first half of 2025, halting deliveries such as Nvidia's H200 to Chinese clients. This staffing crisis creates a critical bottleneck in the enforcement of U.S. export controls on advanced technology, directly impacting the global AI hardware supply chain. The delays hinder Chinese firms' access to cutting-edge AI chips like the H200, potentially affecting their AI development timelines, while also creating uncertainty and financial implications for major U.S. chipmakers like Nvidia and AMD. Beyond staff shortages, delays are exacerbated by increased regulatory complexity, internal management changes, and the fact that Deputy Secretary of Commerce Jeffrey Kessler insists on reviewing nearly every license application personally. The BIS has not released its annual reports for FY2024 and FY2025, forcing the chip industry to rely on unofficial data to assess application progress.

telegram · zaihuapd · Apr 13, 15:25

**Background**: The Bureau of Industry and Security (BIS) is a U.S. Department of Commerce agency responsible for advancing national security and foreign policy through export controls on "dual-use" technologies—items with both civilian and military applications. Since 2018, the U.S. has progressively tightened export controls on advanced semiconductors to China to maintain a technological lead and slow China's development of competitive AI and computing capabilities. The NVIDIA H200 is a high-performance GPU based on the Hopper architecture, designed to supercharge generative AI and high-performance computing workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://www.congress.gov/crs-product/R48642">U.S. Export Controls and China: Advanced Semiconductors</a></li>
<li><a href="https://resources.nvidia.com/en-us-gpu-resources/hpc-datasheet-sc23">NVIDIA H200 GPU Datasheet</a></li>
<li><a href="https://govfacts.org/government/federal/agencies/commerce/a-step-by-step-guide-to-applying-for-a-bis-export-license/">A Step-by-Step Guide to Applying for a BIS Export License</a></li>

</ul>
</details>

**Tags**: `#Geopolitics`, `#AI Hardware`, `#Supply Chain`, `#Export Controls`, `#Nvidia`

---

<a id="item-8"></a>
## [Bryan Cantrill argues LLMs lack human laziness, leading to bloated systems](https://simonwillison.net/2026/Apr/13/bryan-cantrill/#atom-everything) ⭐️ 7.0/10

In a blog post, software engineer Bryan Cantrill argues that large language models inherently lack the human virtue of laziness, which he defines as the incentive to optimize for future time. He contends that because work costs nothing to an LLM, it will happily create layered systems of garbage without the natural human drive to develop crisp, efficient abstractions. This perspective highlights a fundamental limitation in AI-assisted software development, suggesting that unchecked LLM use could lead to increasingly large and inefficient systems rather than better ones. It forces developers and organizations to consider the optimization incentives—or lack thereof—in their AI tools, potentially shifting focus from vanity metrics like lines of code to genuine system quality and maintainability. Cantrill specifically warns that LLMs, lacking the need to optimize for anyone's future time, will appeal to "perverse vanity metrics" at the cost of everything that matters in software. His argument is rooted in the observation that human laziness is a virtue that forces the creation of crisp abstractions to avoid wasting time on clunky implementations.

rss · Simon Willison · Apr 13, 02:44

**Background**: Bryan Cantrill is a well-known software engineer recognized for his work on DTrace at Sun Microsystems and his commentary on systems software. A "layered cake" or "layercake" in software architecture refers to a design with multiple tiers (like presentation, logic, and data layers), which can become bloated if not carefully managed. "Vanity metrics" are measurements that look impressive (e.g., lines of code, number of commits) but do not necessarily correlate with real value or quality in software development.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bryan_Cantrill">Bryan Cantrill - Wikipedia</a></li>
<li><a href="https://masterlwa.medium.com/layered-architecture-the-delicious-cake-of-software-architecting-5102e3f80202">Layered Architecture: The Delicious Cake of Software Architecting | by Lakindu Widuranga Alwis | Medium</a></li>
<li><a href="https://www.baytechconsulting.com/blog/future-developer-productivity-metrics-2026">The Future of Developer Productivity: Metrics That Matter</a></li>

</ul>
</details>

**Tags**: `#llms`, `#software-engineering`, `#abstraction`, `#optimization`, `#philosophy`

---

<a id="item-9"></a>
## [Durov Challenges WhatsApp's Default Encryption Claims, Reveals Unencrypted Cloud Backups](https://t.me/zaihuapd/40826) ⭐️ 7.0/10

Telegram founder Pavel Durov has publicly criticized WhatsApp's claims of 'default end-to-end encryption,' revealing that over 95% of private messages are stored unencrypted in cloud backups on Apple or Google servers. Furthermore, Durov stated that WhatsApp collects and shares user metadata with third parties, contrasting this with Telegram's claim of never having disclosed user message data. This matters because WhatsApp's default encryption claims may mislead its over two billion users about the true privacy of their communications, creating a false sense of security. The widespread practice of storing backups in plaintext on third-party servers exposes vast amounts of sensitive personal data to potential access by cloud providers, governments, or hackers, fundamentally undermining the purpose of end-to-end encryption. A critical technical caveat is that even if a user enables encrypted backups, their chat history remains unencrypted if the other participant in the conversation has not enabled the same setting, as messages are stored in each user's individual cloud backup. The content also highlights that Apple and Google reportedly disclose WhatsApp backup data to third parties thousands of times per year.

telegram · zaihuapd · Apr 12, 16:07

**Background**: End-to-end encryption (E2EE) is a communication system where only the communicating users can read the messages, preventing potential eavesdroppers like telecom providers, internet providers, or the service provider itself from accessing the cryptographic keys needed to decrypt the conversation. Metadata refers to data about the communication (e.g., who talked to whom, when, for how long, from which location), which can reveal sensitive patterns and relationships even if the message content is encrypted. Cloud backups are copies of app data (like chat histories) automatically stored by services like iCloud or Google Drive to allow data restoration across devices.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/端到端加密">端到端加密 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.cngold.com.cn/202308107064565348.html">什么是元数据隐私及其为何重要？-新闻资讯-中金网</a></li>

</ul>
</details>

**Tags**: `#encryption`, `#privacy`, `#messaging-apps`, `#security`, `#data-protection`

---

<a id="item-10"></a>
## [Third-party benchmark reports Claude Opus 4.6 hallucination rate surged, ranking drops from 2nd to 10th](https://www.bridgebench.ai/) ⭐️ 7.0/10

The AI evaluation platform BridgeMind reported that Claude Opus 4.6's accuracy on the BridgeBench hallucination benchmark dropped from 83.3% (ranking 2nd) last week to 68.3% (ranking 10th), a decrease of about 15 percentage points. The platform suggests the model's reasoning capabilities may have been weakened and advises users to delay deployment until a new version is officially released. This significant performance regression in a flagship AI model raises serious questions about model stability and the reliability of deployment decisions for AI practitioners. It highlights the critical role of independent, ongoing benchmarking in tracking model performance over time, especially for high-stakes applications like coding where hallucinations can introduce critical errors. The report indicates a 98% increase in hallucinations for Claude Opus 4.6 on this specific benchmark. Notably, other top models on the BridgeBench leaderboard maintained accuracy rates above 80% during the same period, and Anthropic has not yet publicly responded to these findings.

telegram · zaihuapd · Apr 13, 05:00

**Background**: BridgeBench is a comprehensive AI coding model benchmarking platform built by BridgeMind. It evaluates models across multiple categories including hallucination resistance, which measures a model's tendency to generate incorrect or fabricated information. Claude Opus is Anthropic's flagship large language model series, with version 4.6 being promoted for its exceptional reasoning and state-of-the-art coding capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bridgemind.ai/bridgebench">BridgeBench — Now at bridgebench.ai - bridgemind.ai</a></li>
<li><a href="https://tech.yahoo.com/ai/claude/articles/viral-bridgebench-post-claims-claude-131318087.html">Viral BridgeBench Post Claims Claude Opus 4.6 Was ‘Nerfed ...</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-6">Claude Opus 4.6 \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI Evaluation`, `#Claude`, `#Hallucination`, `#Benchmarking`, `#Model Performance`

---

<a id="item-11"></a>
## [Cloudflare Data Shows AI Giants Disrupting Web's Economic Balance, Anthropic's 'Crawl-to-Refer' Ratio Most Extreme](https://www.businessinsider.com/ai-bots-strip-mining-web-anthropic-leads-ethical-claude-2026-4) ⭐️ 7.0/10

Cloudflare data reveals a severe imbalance in the web ecosystem, where AI companies, particularly Anthropic, crawl web content at extremely high rates but send almost no traffic back to source sites. Anthropic's crawl-to-referral ratio is an extreme 8800:1, meaning it sends only one visitor for every 8800 pages crawled, far worse than OpenAI's 993:1 ratio. This 'take without giving' behavior threatens the traditional 'grand bargain' of the web, where crawlers index content in exchange for driving valuable human traffic to publishers. As generative AI chatbots provide answers directly instead of linking to sources, website owners bear the cost of crawler traffic while losing the monetization potential from referrals, potentially undermining the economic engine that supports information sharing on the internet. The data suggests this is a fundamental difference in business model, as Anthropic's ClaudeBot operates primarily as a training data crawler for its AI model, unlike search engines like Google which have a balanced ratio. While Anthropic has questioned the methodology, the industry trend shows a clear deterioration in the crawl-to-refer ratio for AI companies compared to traditional search engines.

telegram · zaihuapd · Apr 13, 10:36

**Background**: Web crawlers are automated programs that systematically browse the internet to index content, traditionally used by search engines. The traditional economic model of the web involves a reciprocal exchange: websites allow crawlers to index their content, and in return, search engines send human visitors (traffic) back through search results, which publishers can monetize. Generative AI companies now use similar crawlers to gather vast amounts of web data to train their large language models (LLMs), but their products (like chatbots) are designed to provide synthesized answers directly, reducing the need for users to visit the original source websites.

<details><summary>References</summary>
<ul>
<li><a href="https://www.businessinsider.com/anthropic-openai-google-perplexity-microsoft-mistral-crawling-web-referrals-cloudflare-2026-1">Anthropic, OpenAI Crawl the Web Even More, and Give Little ...</a></li>
<li><a href="https://seomator.com/blog/crawl-to-refer-ratio-ai-crawlers-llm-bots">GEO Data Report 2026: Which AI Crawlers & LLM Bots Take the ...</a></li>
<li><a href="https://www.eyerys.com/articles/news/anthropic-has-highest-crawl-refer-ratio-threatens-future-web-says-cloudflare">Anthropic Has The Highest Crawl-To-Refer Ratio, Threatens The ...</a></li>

</ul>
</details>

**Tags**: `#AI Ethics`, `#Web Crawling`, `#Internet Economics`, `#Cloudflare`, `#Generative AI`

---