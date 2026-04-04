---
layout: default
title: "Horizon Summary: 2026-04-04 (EN)"
date: 2026-04-04
lang: en
---

> From 29 items, 13 important content pieces were selected

---

1. [AI Agents Will Soon Automate Most Vulnerability Research](#item-1) ⭐️ 9.0/10
2. [vLLM v0.19.0 released with Gemma 4 support, zero-bubble async scheduling, and major performance optimizations.](#item-2) ⭐️ 8.0/10
3. [AI-generated vulnerability reports flood Linux kernel security list, overwhelming maintainers](#item-3) ⭐️ 8.0/10
4. [Linux Kernel Maintainer Reports AI-Generated Security Reports Have Become Useful](#item-4) ⭐️ 8.0/10
5. [Axios supply chain attack used targeted social engineering against maintainer](#item-5) ⭐️ 8.0/10
6. [MIIT Warns of High-Risk Apple iOS Vulnerability, Urges Immediate Update](#item-6) ⭐️ 8.0/10
7. [Elon Musk Reportedly Requires Banks in SpaceX IPO to Buy Grok Subscriptions](#item-7) ⭐️ 8.0/10
8. [Viral clip highlights cognitive costs of AI coding agents](#item-8) ⭐️ 7.0/10
9. [Cursor Releases Version 3, a Unified Workspace for AI Agent Development](#item-9) ⭐️ 7.0/10
10. [Google Vids integrates Veo 3.1, offering free AI video generation to all users](#item-10) ⭐️ 7.0/10
11. [American Humanoid Robots Rely on Chinese Technology for Critical Internal Components](#item-11) ⭐️ 7.0/10
12. [LinkedIn allegedly scans browser extensions and shares data with third parties without consent](#item-12) ⭐️ 7.0/10
13. [Researchers Reverse Engineer Claude Code's Request Signing, Bypass Bun Runtime to Forge Headers](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [AI Agents Will Soon Automate Most Vulnerability Research](https://simonwillison.net/2026/Apr/3/vulnerability-research-is-cooked/#atom-everything) ⭐️ 9.0/10

Security expert Thomas Ptacek argues that frontier AI models will soon cause a step-function change in vulnerability research, enabling AI agents to automate the discovery of zero-day exploits by brute-forcing source code analysis. This transformation is predicted to occur within months, fundamentally altering the practice and economics of exploit development. This matters because it represents a paradigm shift in cybersecurity, where AI automation could dramatically lower the barrier to finding critical vulnerabilities, potentially flooding the market with zero-days and forcing a complete rethinking of software security practices. The economics of both offensive security research and defensive patching will be fundamentally disrupted. The analysis highlights that LLMs are exceptionally well-suited for vulnerability research because they encode vast knowledge of code correlations and documented bug classes like stale pointers and integer mishandling. The agent-based approach combines this baked-in knowledge with brute-force pattern matching and constraint-solving capabilities that can run indefinitely without fatigue.

rss · Simon Willison · Apr 3, 23:59

**Background**: Vulnerability research involves finding security flaws in software before attackers do, with zero-day vulnerabilities being particularly valuable as they're unknown to vendors and have no patches. LLM agents are AI systems that can autonomously perform complex tasks by breaking them down into steps, using tools, and making decisions. Frontier models refer to the most advanced AI systems currently available, which possess capabilities significantly beyond previous generations.

<details><summary>References</summary>
<ul>
<li><a href="https://sockpuppet.org/blog/2026/03/30/vulnerability-research-is-cooked/">Vulnerability Research Is Cooked — Quarrelsome</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>
<li><a href="https://github.com/NVISOsecurity/cyber-security-llm-agents">GitHub - NVISOsecurity/ cyber - security - llm - agents : A collection of...</a></li>

</ul>
</details>

**Tags**: `#ai-security`, `#vulnerability-research`, `#llm-agents`, `#exploit-development`, `#cybersecurity`

---

<a id="item-2"></a>
## [vLLM v0.19.0 released with Gemma 4 support, zero-bubble async scheduling, and major performance optimizations.](https://github.com/vllm-project/vllm/releases/tag/v0.19.0) ⭐️ 8.0/10

vLLM v0.19.0 has been released, introducing full support for Google's Gemma 4 model architecture and a significant performance enhancement through zero-bubble async scheduling combined with speculative decoding. The release also marks the maturation of Model Runner V2 with piecewise CUDA graphs for pipeline parallelism and introduces a general CPU KV cache offloading mechanism. This release is significant because it directly improves the throughput and efficiency of serving large language models, a critical factor for production AI applications. The combination of zero-bubble scheduling and speculative decoding reduces idle GPU time, while broader model support and architectural enhancements make vLLM a more versatile and powerful inference engine for the ecosystem. The zero-bubble async scheduling feature specifically reduces 'GPU bubbles' in high-throughput serving by allowing the scheduler to prepare the next batch while the GPU is busy. The new CPU KV cache offloading is a pluggable mechanism that moves KV caches from GPU to CPU memory, enabling more potential cache hits and handling larger models or contexts.

github · khluu · Apr 3, 02:19

**Background**: vLLM is a high-throughput and memory-efficient inference and serving engine for large language models (LLMs). Speculative decoding is a technique where a smaller, faster 'draft' model proposes tokens, and a larger 'target' model verifies them, aiming to reduce latency. CUDA graphs are a performance optimization in NVIDIA's CUDA that captures a sequence of kernel launches into a single, replayable unit to reduce launch overhead. Pipeline parallelism is a model parallelism technique that splits a model's layers across multiple GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/">Speculative Decoding - vLLM</a></li>
<li><a href="https://agentnativedev.medium.com/vllm-v0-14-0-async-scheduling-grpc-and-deployability-b042bbe40312">vLLM v0.14.0: Async Scheduling, gRPC, and Deployability | by Agent Native | Medium</a></li>
<li><a href="https://docs.sglang.io/advanced_features/piecewise_cuda_graph.html">Piecewise CUDA Graph — SGLang</a></li>

</ul>
</details>

**Tags**: `#llm-inference`, `#performance-optimization`, `#vllm`, `#model-serving`, `#gpu-acceleration`

---

<a id="item-3"></a>
## [AI-generated vulnerability reports flood Linux kernel security list, overwhelming maintainers](https://simonwillison.net/2026/Apr/3/willy-tarreau/#atom-everything) ⭐️ 8.0/10

Willy Tarreau, a lead developer and Linux kernel maintainer, reports that AI-generated security vulnerability reports to the kernel security list have surged from 2-3 per week two years ago to 5-10 per day in 2026, forcing the team to bring in more maintainers. A new phenomenon of duplicate reports for the same bug, likely from different AI tools, is now occurring daily. This dramatic increase in AI-generated reports represents a significant shift in the vulnerability disclosure landscape, creating a new operational bottleneck for critical open-source infrastructure. It highlights how AI-powered security tools, while effective at finding bugs, can inadvertently strain the human review processes that underpin software security. While Tarreau notes that most of the AI-generated reports are correct, the sheer volume and the emergence of duplicate findings are the primary challenges. The influx has been so significant that it required scaling up the maintainer team to handle the triage and validation workload.

rss · Simon Willison · Apr 3, 21:48

**Background**: The Linux kernel security list is a dedicated mailing list for reporting and discussing security vulnerabilities in the Linux kernel. Willy Tarreau is the lead developer of HAProxy, a widely-used open-source load balancer, and is also an active Linux kernel maintainer. AI-powered vulnerability scanning tools use machine learning and large language models to automatically analyze code for potential security flaws, a practice that has become increasingly common.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/566123/">Opening up kernel security bug handling [LWN.net]</a></li>
<li><a href="https://www.haproxy.com/company/careers">Open Positions - HAProxy Technologies Careers</a></li>

</ul>
</details>

**Tags**: `#security`, `#linux-kernel`, `#ai`, `#vulnerability-management`, `#maintenance`

---

<a id="item-4"></a>
## [Linux Kernel Maintainer Reports AI-Generated Security Reports Have Become Useful](https://simonwillison.net/2026/Apr/3/greg-kroah-hartman/#atom-everything) ⭐️ 8.0/10

Greg Kroah-Hartman, a key Linux kernel maintainer, stated that AI-generated security reports submitted to open-source projects have recently undergone a dramatic shift in quality. He noted that while these reports were previously low-quality 'AI slop,' they have now become accurate and genuinely useful across all open-source projects. This shift matters because it signals that AI tools are maturing from a source of noise to a legitimate aid for securing critical software infrastructure. If AI can reliably identify real vulnerabilities, it could significantly scale up security auditing and reduce the burden on overworked open-source maintainers. Kroah-Hartman pinpointed the change as occurring about a month prior to his March 2026 statement. He emphasized that the improvement is not isolated but is being observed consistently across the entire open-source ecosystem.

rss · Simon Willison · Apr 3, 21:44

**Background**: Greg Kroah-Hartman is a leading maintainer of the Linux kernel, responsible for overseeing parts of the codebase, reviewing patches, and ensuring stability. 'AI slop' is a term for low-quality, often meaningless content generated by AI in high volume, which has been a growing concern in software development as AI agents flood projects with erroneous reports. Open-source projects traditionally rely on community vulnerability disclosures to improve security.

<details><summary>References</summary>
<ul>
<li><a href="https://linuxvox.com/blog/linux-kernal-maintainers/">Linux Kernel Maintainers: A Comprehensive Guide - linuxvox.com</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_slop">AI slop - Wikipedia</a></li>
<li><a href="https://www.axios.com/2026/03/10/ai-agents-spam-the-volunteers-securing-open-source-software">AI agents are flooding open-source maintainers with security reports</a></li>

</ul>
</details>

**Tags**: `#ai-security`, `#open-source`, `#linux-kernel`, `#generative-ai`

---

<a id="item-5"></a>
## [Axios supply chain attack used targeted social engineering against maintainer](https://simonwillison.net/2026/Apr/3/supply-chain-social-engineering/#atom-everything) ⭐️ 8.0/10

The Axios team published a postmortem revealing that a recent supply chain attack, which resulted in a malware-laden release, was executed through a sophisticated social engineering campaign specifically targeting a project maintainer. The attackers, mimicking the UNC1069 threat actor's tactics, created a convincing fake company and used a Slack workspace and Microsoft Teams meeting to trick the maintainer into installing a Remote Access Trojan (RAT). This incident highlights a critical shift in software supply chain attacks, where threat actors now directly target the human maintainers of widely-used open-source libraries rather than just exploiting technical vulnerabilities. It demonstrates that even projects with strong technical security can be compromised through sophisticated social engineering, putting millions of downstream users and applications at risk. The attack was highly tailored, involving a cloned company with fake founder profiles, a realistic Slack workspace with channels and fake team member profiles, and a coordinated MS Teams meeting where the RAT was disguised as a required update. The malicious npm packages were live for approximately 3 hours before being detected and taken down.

rss · Simon Willison · Apr 3, 13:54

**Background**: A software supply chain attack occurs when attackers compromise a third-party component, like an open-source library, to indirectly target all its users. The threat actor group UNC1069, suspected to have North Korean ties, is known for financially motivated attacks and has recently evolved to use AI-enhanced social engineering. Axios is a popular JavaScript HTTP client library used by millions of developers worldwide.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/04/unc1069-social-engineering-of-axios.html">UNC1069 Social Engineering of Axios Maintainer Led to npm ...</a></li>
<li><a href="https://cloud.google.com/blog/topics/threat-intelligence/unc1069-targets-cryptocurrency-ai-social-engineering">UNC 1069 Targets Cryptocurrency Sector with... | Google Cloud Blog</a></li>
<li><a href="https://onymos.com/blog/how-vulnerable-are-you-to-a-supply-chain-attack/">How Vulnerable Are You to a Supply Chain Attack ? - Onymos</a></li>

</ul>
</details>

**Tags**: `#security`, `#supply-chain-attack`, `#social-engineering`, `#open-source`, `#axios`

---

<a id="item-6"></a>
## [MIIT Warns of High-Risk Apple iOS Vulnerability, Urges Immediate Update](https://www.nvdb.org.cn/publicAnnouncement/2040008892420247553) ⭐️ 8.0/10

China's Ministry of Industry and Information Technology (MIIT) Cybersecurity Threat and Vulnerability Information Sharing Platform (NVDB) has issued a warning about an active exploitation of a high-risk vulnerability in Apple devices. The vulnerability affects iPhones and iPads running iOS/iPadOS versions 13.0 through 17.2.1, allowing attackers to implant a Remote Access Trojan (RAT) and gain full system control. This official alert highlights an urgent, widespread security threat that could lead to massive data theft and complete device compromise for millions of users. The involvement of a national cybersecurity authority underscores the severity and real-world exploitation of the flaw, demanding immediate action from both individual users and enterprise administrators. The attack vector involves luring users to malicious webpages via SMS, email, or web poisoning, which then exploits the vulnerability to silently install the RAT. The NVDB specifically advises users to update their systems immediately or apply patches, and to avoid clicking on links from untrusted sources.

telegram · zaihuapd · Apr 3, 11:23

**Background**: The MIIT's NVDB is China's official platform for sharing information on cybersecurity threats and vulnerabilities, similar to databases like CVE. A Remote Access Trojan (RAT) is a type of malware that provides an attacker with administrative control over a compromised device, enabling activities like data theft, surveillance, and further system manipulation. Web poisoning is an attack technique where attackers compromise legitimate websites or create malicious ones to distribute malware.

<details><summary>References</summary>
<ul>
<li><a href="https://www.itiger.com/news/2566671621">防范苹果公司iOS/iPadOS/macOS越界写入高危漏洞 - Tiger Brokers</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/655411571">远控木马详解与防御及APT攻击中的远控 - 知乎 木马程序原理与远程执行技术全解析-CSDN博客 工信部紧急提醒苹果用户_信息化_漏洞_网页 远控木马详解及APT攻击中的远控和防御-百度开发者中心 RAT (Remote Access Trojan ）远程控制木马专题一 | CN-SEC 中文网</a></li>
<li><a href="https://www.163.com/dy/article/KPK1OE650534P59R.html">工信部：有攻击者用短信、邮件或网页投毒等方式，向苹果公司终端产品...</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#vulnerability`, `#apple`, `#ios`, `#government-alert`

---

<a id="item-7"></a>
## [Elon Musk Reportedly Requires Banks in SpaceX IPO to Buy Grok Subscriptions](https://arstechnica.com/tech-policy/2026/04/elon-musk-insists-banks-working-on-spacex-ipo-must-buy-grok-subscriptions/) ⭐️ 8.0/10

According to anonymous sources familiar with confidential negotiations, Elon Musk has required banks, law firms, and audit agencies advising on SpaceX's IPO to purchase subscriptions for xAI's Grok chatbot. Some banks have reportedly agreed to commit tens of millions of dollars to these subscriptions and have begun integrating Grok into their IT systems. This move raises significant questions about potential conflicts of interest and the bundling of unrelated services in a major financial transaction. It could set a precedent for how tech founders leverage high-stakes corporate events to cross-sell other products within their business empires, potentially influencing market practices and regulatory scrutiny. SpaceX reportedly submitted its IPO filing to the SEC this week, just two months after acquiring xAI. The requirement for banks to buy Grok subscriptions appears to be more firmly enforced than a separate, earlier request from Musk for the same banks to advertise on his social media platform X.

telegram · zaihuapd · Apr 4, 00:07

**Background**: SpaceX, Elon Musk's aerospace company, has confidentially filed for an Initial Public Offering (IPO), a process where a private company offers shares to the public for the first time. xAI is Musk's artificial intelligence company, which developed the Grok chatbot; SpaceX recently acquired xAI in a historic deal. Grok is an advanced AI model known for features like real-time web access and reasoning capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.investopedia.com/spacex-filed-to-go-public-every-step-between-now-and-when-you-can-buy-shares-11940905">SpaceX Filed to Go Public—Here's Every Step Between Now and When You Can Buy Shares</a></li>
<li><a href="https://markets.financialcontent.com/stocks/article/marketminute-2026-3-30-the-galactic-merger-spacex-consolidates-xai-in-125-trillion-deal">The Galactic Merger: SpaceX Consolidates xAI in $1.25 ...</a></li>
<li><a href="https://guptadeepak.com/research/grok-ai-fundamentals/">Grok AI - Core Concepts, Capabilities, Technical Foundation</a></li>

</ul>
</details>

**Tags**: `#business`, `#tech-policy`, `#artificial-intelligence`, `#ipo`, `#elon-musk`

---

<a id="item-8"></a>
## [Viral clip highlights cognitive costs of AI coding agents](https://simonwillison.net/2026/Apr/3/cognitive-cost/#atom-everything) ⭐️ 7.0/10

A 48-second clip from Simon Willison's podcast appearance on Lenny Rachitsky's show, discussing the cognitive costs of using AI coding agents, went viral on Twitter/X with over 1.1 million views. The clip was extracted from a full 1 hour 40 minute conversation about the implications of these tools. This discussion matters because as AI coding agents like GitHub Copilot, Cursor, and Claude Code become ubiquitous in software development, understanding their cognitive impact on developers is crucial for long-term productivity and skill development. The viral attention indicates widespread developer concern about how these tools might affect critical thinking and problem-solving abilities. The viral clip specifically addresses the concept of 'cognitive debt' or 'cognitive cost' - the idea that over-reliance on AI coding assistance may cause developers' own problem-solving and critical thinking abilities to atrophy over time. This discussion is part of a broader conversation about AI ethics and the long-term implications of agentic engineering in software development.

rss · Simon Willison · Apr 3, 23:57

**Background**: AI coding agents are tools that assist developers by generating, completing, or debugging code using large language models. Popular examples include GitHub Copilot, Cursor, Claude Code, and Devin. These tools have revolutionized developer workflows but raise questions about their cognitive impact. The term 'cognitive cost' refers to potential negative effects on human cognitive abilities from over-reliance on AI assistance, similar to concerns raised by Harvard professor Avi Loeb about AI tools causing critical thinking abilities to atrophy.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/agents/coding">Coding Agents Comparison: Cursor, Claude Code, GitHub Copilot ...</a></li>
<li><a href="https://futurism.com/artificial-intelligence/harvard-avi-loeb-ai">Harvard Professor Says AI Users Are Losing Cognitive Abilities - Futurism</a></li>
<li><a href="https://www.media.mit.edu/publications/your-brain-on-chatgpt/">Your Brain on ChatGPT: Accumulation of Cognitive Debt when Using an ...</a></li>

</ul>
</details>

**Tags**: `#ai-ethics`, `#coding-agents`, `#developer-productivity`, `#ai-tools`, `#software-engineering`

---

<a id="item-9"></a>
## [Cursor Releases Version 3, a Unified Workspace for AI Agent Development](https://cursor.com/blog/cursor-3) ⭐️ 7.0/10

Cursor has officially launched Cursor 3, a major update that repositions the tool as a unified workspace designed specifically for AI agents. The new version features a completely redesigned, agent-centric interface, introduces multi-repository workspace support, and enables hybrid workflows that allow seamless handoff between local and cloud-based agent sessions. This release is significant as it represents a shift from Cursor being primarily an AI-assisted code editor to a comprehensive platform for orchestrating AI agents in software development. It directly addresses the growing need for tools that can manage complex, multi-repository projects and support persistent, long-running AI agents that work across different environments, which is a key trend in agentic AI development. The hybrid workflow allows developers to start an agent session locally for editing and testing, then move it to the cloud to continue running even when offline or switching tasks. The update also includes a new diff view for faster editing and reviewing changes, and retains core Git operations like staging, committing, and managing pull requests.

telegram · zaihuapd · Apr 3, 02:00

**Background**: Cursor is an AI-powered integrated development environment (IDE) built to enhance developer productivity through features like AI code completion, chat-based assistance, and automated edits. It is often compared to VS Code with GitHub Copilot. AI agents in this context refer to more autonomous AI assistants that can perform complex, multi-step development tasks, such as implementing features or fixing bugs across an entire codebase. The Model Context Protocol (MCP) is an open standard that enables these AI agents to safely connect to and use external tools and data sources, which Cursor treats as a first-class capability.

<details><summary>References</summary>
<ul>
<li><a href="https://cursor.com/">Cursor : The best way to code with AI</a></li>
<li><a href="https://www.devtoolsacademy.com/blog/cursor-vs-claudecode/">Cursor vs Claude Code: A Comprehensive Comparison</a></li>
<li><a href="https://howaiworks.ai/blog/cursor-3-unified-workspace-agents">Introducing Cursor 3: A Unified Agentic Workspace - howaiworks.ai</a></li>

</ul>
</details>

**Tags**: `#AI-assisted-development`, `#developer-tools`, `#software-engineering`, `#cursor`, `#AI-agents`

---

<a id="item-10"></a>
## [Google Vids integrates Veo 3.1, offering free AI video generation to all users](https://www.techradar.com/ai-platforms-assistants/google-is-pushing-ai-video-into-ordinary-life-just-as-openai-pulls-sora-back) ⭐️ 7.0/10

Google has integrated its state-of-the-art Veo 3.1 AI video generation model into its browser-based video creation tool, Google Vids, and is now offering a free monthly quota of 10 video generations to all Google account holders. The update also adds Lyria 3 music generation models for creating 30-second to 3-minute soundtracks and introduces customizable digital avatars, though the music feature is limited to paid AI Pro and Ultra subscribers. This move significantly democratizes access to high-quality AI video generation, making a powerful creative tool freely available to the general public and contrasting with OpenAI's more restrictive approach to its Sora model. By embedding these capabilities into a widely accessible platform like Google Vids, Google is pushing AI video from a specialized tool into everyday creative workflows for presentations, social media, and personal projects. The free tier for personal users is capped at 10 generations per month, while paid Google AI Ultra and Workspace AI Ultra subscribers receive a significantly higher quota of up to 1,000 Veo generations monthly. The integrated Lyria 3 and Lyria 3 Pro models can generate music with vocals and lyrics, but this advanced feature remains a premium offering for paying customers.

telegram · zaihuapd · Apr 3, 05:23

**Background**: Google Veo 3.1 is Google's latest and most advanced AI video generation model, capable of creating high-quality, 8-second videos with sound from text or images, and supporting outputs up to 4K resolution in various aspect ratios. Lyria 3 is Google DeepMind's flagship AI music generation model family, which can create professional-grade audio clips, including tracks with realistic vocals and auto-generated lyrics, from text, image, or video prompts. Google Vids is a web-based AI-assisted video creation tool within Google Workspace, designed to help users quickly produce videos for presentations and other content.

<details><summary>References</summary>
<ul>
<li><a href="https://aistudio.google.com/models/veo-3">Veo 3 | Google AI Studio</a></li>
<li><a href="https://deepmind.google/models/lyria/">Lyria 3 — Google DeepMind</a></li>

</ul>
</details>

**Tags**: `#AI Video Generation`, `#Google AI`, `#Veo 3.1`, `#Creative Tools`, `#AI Democratization`

---

<a id="item-11"></a>
## [American Humanoid Robots Rely on Chinese Technology for Critical Internal Components](https://www.wsj.com/tech/under-the-skin-of-americas-humanoid-robots-chinese-technology-27dd4fdf) ⭐️ 7.0/10

A Wall Street Journal report reveals that American humanoid robots, including Disney's "Olaf" robot and Tesla's Optimus, are increasingly dependent on Chinese suppliers for critical components like motors, joints, magnets, and sensors. The report also notes that China plans to launch 28 humanoid robot models in 2025, nearly three times the number from US companies, and that Chinese supply chains could reduce manufacturing costs by up to two-thirds. This dependency creates a significant supply chain vulnerability for a cutting-edge technology sector central to future automation and AI strategy. It highlights a strategic weakness for US technological development and has prompted bipartisan legislative action in the US Congress to assess competitiveness and supply chain risks. Specific examples include Disney's "Olaf" robot using components from China's Unitree Robotics, and Tesla collaborating with Chinese suppliers for Optimus mass production. Joint actuators, a key component sourced from China, can account for 30–50% of a humanoid robot's bill of materials (BOM), making cost and supply critical.

telegram · zaihuapd · Apr 3, 08:55

**Background**: Humanoid robots are advanced machines designed to mimic human form and movement, with applications ranging from manufacturing to customer service. Key to their function are internal components like actuators (which provide movement at joints) and sensors (which provide perception). Companies like Tesla (with Optimus) and Unitree Robotics are major players in developing these robots. The supply chain for the sophisticated components required is global and complex.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unitree_Robotics">Unitree Robotics - Wikipedia</a></li>
<li><a href="https://interactanalysis.com/insight/joint-actuators-the-fundamental-component-for-humanoid-robots-power-and-dexterity/">Joint Actuators: Powering the Future of Humanoid Robotics</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#supply-chain`, `#geopolitics`, `#manufacturing`, `#ai-hardware`

---

<a id="item-12"></a>
## [LinkedIn allegedly scans browser extensions and shares data with third parties without consent](https://cybernews.com/privacy/linkedin-surveillance-browsergate/?utm_source=flipboard&amp;utm_content=CyberNews_com%2Fmagazine%2FLatest+cybersecurity+news) ⭐️ 7.0/10

A new report dubbed 'BrowserGate' alleges that Microsoft's LinkedIn uses hidden JavaScript scripts on its website to scan visitors' browsers for over 6,000 installed extensions and collect device data. This data, which can reveal sensitive information like religious beliefs or job-seeking status, is then encrypted and sent to LinkedIn's servers, potentially affecting 405 million users, and is shared with third-party companies like HUMAN Security without obtaining proper user consent. This practice represents a significant privacy intrusion, as the scanned data can be used to build detailed user profiles that infer sensitive personal attributes without explicit permission. It raises serious concerns about corporate surveillance and potential violations of data protection regulations like the GDPR, which typically requires explicit user consent for such processing. The scanning targets over 6,000 browser extensions and more than 200 competing tools, collecting data that could indicate a user's religion, political leanings, health status, or job-seeking activity. LinkedIn has not disclosed this practice to users, nor has it obtained the explicit consent required under the EU's General Data Protection Regulation (GDPR) for such data sharing with third parties.

telegram · zaihuapd · Apr 3, 12:09

**Background**: Browser extensions are small software programs that add features or modify the functionality of a web browser. While useful, they can pose security and privacy risks, as the extensions a user installs can reveal personal interests, habits, and even sensitive attributes. The GDPR is a comprehensive EU regulation that governs data protection and privacy, requiring organizations to obtain clear and affirmative consent from individuals before processing their personal data, especially for purposes like profiling or sharing with third parties.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/linkedin-secretely-scans-for-6-000-plus-chrome-extensions-collects-data/">LinkedIn secretely scans for 6,000+ Chrome extensions ...</a></li>
<li><a href="https://appleinsider.com/articles/26/04/03/microsofts-linkedin-is-scanning-installed-browser-extensions-without-user-permission">Microsoft's LinkedIn is scanning installed browser extensions ...</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#data-protection`, `#gdpr`, `#linkedin`, `#browser-security`

---

<a id="item-13"></a>
## [Researchers Reverse Engineer Claude Code's Request Signing, Bypass Bun Runtime to Forge Headers](https://a10k.co/b/reverse-engineering-claude-code-cch.html) ⭐️ 7.0/10

A technical analysis published on April 2, 2026, details how researchers reverse-engineered the proprietary request signing mechanism used by Anthropic's Claude Code. They discovered that the `cch` integrity check header is computed by the embedded Bun runtime using the xxHash64 algorithm on a specific JSON structure, and they successfully created a Python proof-of-concept to forge these signatures without relying on Bun. This matters because it exposes the inner workings of a key security and feature-gating mechanism in a major AI coding assistant. The ability to forge signatures could allow developers to bypass intended restrictions, such as enabling 'fast mode' or other gated features, and highlights that the mechanism is designed more for billing attribution and feature control than for strong access security. The `cch` hash is calculated by the Bun runtime's native fetch on a complete JSON request body containing a `cch=00000` placeholder. The `cc_version` suffix is derived from SHA-256 hashing specific characters from the first user message, a built-in salt, and a version number. The analysis suggests this scheme is not a robust access control but rather a mechanism for tracking usage and gating premium features.

telegram · zaihuapd · Apr 3, 15:00

**Background**: Claude Code is an AI-powered coding assistant developed by Anthropic. It communicates with Anthropic's backend APIs using proprietary headers for authentication and request integrity. Bun is a fast JavaScript runtime written in Zig, often used for its performance. The `cch` header is a request integrity check value; incorrect values cause API requests to be rejected. xxHash64 is an extremely fast non-cryptographic hash algorithm often used for checksums.

<details><summary>References</summary>
<ul>
<li><a href="https://rexai.top/en/ai/claude-code/2026-04-02-reverse-engineering-claude-code-cch/">Reverse Engineering Claude Code's API Request Signing</a></li>
<li><a href="https://bun.com/docs/runtime">Bun Runtime - Bun</a></li>
<li><a href="https://github.com/Cyan4973/xxHash">xxHash - Extremely fast hash algorithm - GitHub What's cch? Reverse Engineering Claude Code's Request Signing XXHash Algorithm Implementation | ceph/xxHash | DeepWiki pyspark.sql.functions.xxhash64 — PySpark 4.1.1 documentation XxHash64 Class (System.IO.Hashing) | Microsoft Learn XXHash Algorithm Implementation | ceph/xxHash | DeepWiki xxHash : XXH64 family XXHash Algorithm Implementation | ceph/xxHash | DeepWiki XXH64 family - xxHash</a></li>

</ul>
</details>

**Tags**: `#reverse-engineering`, `#api-security`, `#anthropic`, `#claude-code`, `#authentication`

---