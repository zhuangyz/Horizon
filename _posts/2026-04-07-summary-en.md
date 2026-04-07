---
layout: default
title: "Horizon Summary: 2026-04-07 (EN)"
date: 2026-04-07
lang: en
---

> From 33 items, 10 important content pieces were selected

---

1. [Researchers discover undocumented bug in Apollo 11 guidance computer code using formal verification.](#item-1) ⭐️ 8.0/10
2. [OpenAI, Anthropic, and Google Unite to Combat AI Model Copying by Chinese Competitors](#item-2) ⭐️ 8.0/10
3. [Anthropic signs major compute deal with Google and Broadcom for next-gen TPUs starting 2027](#item-3) ⭐️ 8.0/10
4. [Cursor's 'Warp Decode' Boosts MoE Inference Throughput by 1.84x on Blackwell GPUs](#item-4) ⭐️ 8.0/10
5. [Apple Seeks Supreme Court Review of App Store Fee Ruling, Secures Stay](#item-5) ⭐️ 8.0/10
6. [GitHub Issue Reports 67% Drop in Claude Code Thinking Depth, Team Attributes to Parameter Tuning](#item-6) ⭐️ 8.0/10
7. [Artemis II Crew Breaks 54-Year-Old Record for Farthest Human Spaceflight from Earth](#item-7) ⭐️ 8.0/10
8. [Tesla officially adapts its app for Huawei's HarmonyOS, becoming the first major overseas automaker to join the ecosystem.](#item-8) ⭐️ 8.0/10
9. [New Yorker Investigation Alleges Pattern of Deception by OpenAI CEO Sam Altman](#item-9) ⭐️ 8.0/10
10. [Telegram Enables Direct Bot-to-Bot Communication for AI Agent Collaboration](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Researchers discover undocumented bug in Apollo 11 guidance computer code using formal verification.](https://www.juxt.pro/blog/a-bug-on-the-dark-side-of-the-moon/) ⭐️ 8.0/10

Researchers at JUXT applied formal verification techniques to the reverse-engineered Apollo Guidance Computer (AGC) code and discovered a previously undocumented bug related to the LGYRO LOCK LEAK routine. This bug could have theoretically caused a memory leak in the gyroscope lock logic, though it was never triggered during the actual Apollo 11 mission. This discovery demonstrates the power of modern formal verification techniques in analyzing and securing historically significant, safety-critical software systems, even decades after their creation. It also highlights the ongoing value of studying legacy systems, not just for historical preservation but for improving contemporary software engineering practices in aerospace and other high-stakes domains. The bug was found by creating a formal specification (model) of the code's intended behavior and then proving that the actual code did not always satisfy this specification. A key caveat is that the specification was derived from the reverse-engineered code itself, not from the original NASA requirements documents, which raises questions about the circularity of the finding as noted in community discussion.

hackernews · henrygarner · Apr 7, 10:25

**Background**: The Apollo Guidance Computer (AGC) was the digital computer installed on the Apollo Command and Lunar Modules, responsible for guidance, navigation, and control during the Moon landings. Formal verification is a mathematical approach to proving or disproving the correctness of software or hardware systems against a formal specification, often used in safety-critical applications. Reverse engineering is the process of analyzing a system to understand its design and function, often applied to legacy software when original documentation is scarce.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apollo_Guidance_Computer">Apollo Guidance Computer - Wikipedia</a></li>
<li><a href="https://extropy-io.medium.com/using-formal-verification-techniques-when-auditing-2cccb739a36d">Using Formal Verification techniques when auditing | Medium</a></li>
<li><a href="https://www.apriorit.com/dev-blog/732-reverse-engineering-automation-evolution">The Evolution of Reverse Engineering: From Manual ... - Apriorit Reverse Engineering: A Roadmap - UCL Computer Science Reverse Engineering Approach - an overview - ScienceDirect Data Reverse Engineering: A Historical Survey - GNU Reverse Engineering Through History: From Stone Tools to CT ... Reverse Engineering : A Roadmap - UCL Computer Science Reverse Engineering : A Roadmap - UCL Computer Science Reverse engineering - Wikipedia Reverse engineering - Wikipedia History of Reverse Engineering | Dan's Docs - GitHub Pages</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed, with interest in the technical verification method but skepticism about the reverse-engineering approach. Some commenters recommend related historical preservation efforts, like the CuriousMarc YouTube channel. Others critique the article's dramatic speculation about the bug's potential impact, noting that astronauts were trained to handle resets. A key technical debate centers on whether deriving specifications from the code, rather than original requirements, undermines the finding's validity.

**Tags**: `#historical-software`, `#formal-verification`, `#space-technology`, `#reverse-engineering`, `#software-bugs`

---

<a id="item-2"></a>
## [OpenAI, Anthropic, and Google Unite to Combat AI Model Copying by Chinese Competitors](https://www.bloomberg.com/news/articles/2026-04-06/openai-anthropic-google-unite-to-combat-model-copying-in-china) ⭐️ 8.0/10

OpenAI, Anthropic, and Google have initiated a rare collaboration through the Frontier Model Forum to share information on combating 'adversarial distillation,' a technique used to extract and replicate the capabilities of their advanced AI models. This move specifically aims to counter unauthorized copying efforts by Chinese competitors, which the U.S. companies view as a threat to their intellectual property and national security. This collaboration marks a significant shift where leading U.S. AI firms are setting aside competitive rivalries to address a common strategic threat, potentially reshaping the global AI competitive landscape. It highlights the escalating tension between technological innovation, intellectual property protection, and national security concerns in the AI race between the U.S. and China. OpenAI has confirmed its participation and referenced a recent memo to the U.S. Congress, specifically alleging that DeepSeek attempted to 'free-ride' on capabilities developed by OpenAI and other U.S. labs. However, the information sharing is currently limited, as the companies are uncertain about what can be shared under existing antitrust guidelines and are seeking clearer boundaries from the U.S. government.

telegram · zaihuapd · Apr 7, 01:27

**Background**: The Frontier Model Forum is an industry body launched in 2023 by Anthropic, Google, Microsoft, and OpenAI, focused on ensuring the safe and responsible development of frontier AI models. 'Adversarial distillation' or model extraction is a security concern where an attacker uses a model's outputs to train a new, functionally similar model, potentially stealing intellectual property and undermining the original developer's competitive advantage. This technique can be used to create cheaper, competitive clones of advanced models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.frontiermodelforum.org/">Frontier Model Forum</a></li>
<li><a href="https://www.frontiermodelforum.org/issue-briefs/issue-brief-adversarial-distillation/">Adversarial Distillation - Frontier Model Forum</a></li>

</ul>
</details>

**Tags**: `#AI Ethics`, `#Geopolitics`, `#Intellectual Property`, `#Industry Collaboration`, `#Model Security`

---

<a id="item-3"></a>
## [Anthropic signs major compute deal with Google and Broadcom for next-gen TPUs starting 2027](https://www.anthropic.com/news/google-broadcom-partnership-compute) ⭐️ 8.0/10

Anthropic announced a multi-gigawatt compute partnership with Google and Broadcom to secure next-generation Tensor Processing Unit (TPU) capacity, with the majority of this new capacity scheduled to come online starting in 2027. The company also revealed its annualized revenue run rate has surpassed $30 billion for 2026, and its enterprise customer base spending over $1 million annually has doubled to over 1,000. This deal represents Anthropic's largest compute commitment to date and is a strategic move to secure the massive, specialized hardware capacity required for training future generations of its Claude AI models. It underscores the intensifying competition in AI infrastructure, where leading AI companies are forming deep partnerships with chip designers and cloud providers to lock in long-term supply and gain performance advantages. The new TPU capacity will primarily be deployed in the United States, aligning with Anthropic's prior commitment to invest in U.S. computing infrastructure. Despite this new Google/Broadcom deal, Anthropic stated it will continue using a multi-vendor strategy that includes AWS Trainium and NVIDIA GPUs, with Amazon remaining a primary cloud and training partner.

telegram · zaihuapd · Apr 7, 02:30

**Background**: Tensor Processing Units (TPUs) are Google's custom-developed application-specific integrated circuits (ASICs) used to accelerate machine learning workloads, particularly for training large AI models. Broadcom is a major semiconductor company that often partners with tech firms on custom chip design, including the high-speed interconnects crucial for linking many chips together in AI training clusters. In the AI accelerator market, TPUs compete with alternatives like NVIDIA's GPUs and AWS's Trainium chips, each offering different performance, cost, and ecosystem trade-offs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ankursnewsletter.com/p/google-tpus-vs-aws-trainium-and-inferentia">Google TPUs vs. AWS Trainium & Inferentia vs. NVIDIA GPUs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Broadcom">Broadcom - Wikipedia</a></li>
<li><a href="https://overcentral.com/en/anthropic-partners-with-google-and-broadcom-on-ai-chips/">Anthropic, Google, Broadcom Partner on AI Chips</a></li>

</ul>
</details>

**Tags**: `#AI Infrastructure`, `#Cloud Computing`, `#TPU`, `#Anthropic`, `#Hardware`

---

<a id="item-4"></a>
## [Cursor's 'Warp Decode' Boosts MoE Inference Throughput by 1.84x on Blackwell GPUs](https://cursor.com/blog/warp-decode) ⭐️ 8.0/10

Cursor introduced a novel inference optimization method called 'warp decode' for Mixture-of-Experts (MoE) models, which reorganizes computation from being 'expert-centric' to 'output-centric' during autoregressive decoding. This approach eliminates five data rearrangement steps from the traditional eight-stage pipeline and compresses the entire MoE layer computation into just two kernels. This optimization significantly improves inference efficiency for MoE models, which are increasingly popular for scaling large language models with less compute. The claimed 1.84x throughput improvement on Blackwell GPUs addresses a critical bottleneck in real-time AI applications where small-batch, low-latency decoding is essential. The optimization specifically targets small-batch decode scenarios on Blackwell GPUs and is not a general replacement for expert-centric execution, which remains advantageous for prefill and large-batch inference. In testing on NVIDIA B200 GPUs with Qwen-3-style models, the method achieved 3.95 TB/s sustained bandwidth at batch size 32 (approximately 58% of peak measured bandwidth) while also improving numerical precision by eliminating intermediate activation quantization.

telegram · zaihuapd · Apr 7, 04:00

**Background**: Mixture-of-Experts (MoE) is a neural network architecture where different specialized sub-networks (experts) handle different inputs, activated via a routing mechanism, enabling models to scale efficiently. Autoregressive decoding is the sequential token-by-token generation process used by models like GPT during inference, which can become a bottleneck. GPU kernel optimization involves restructuring low-level computation routines to better utilize hardware parallelism and memory bandwidth.

<details><summary>References</summary>
<ul>
<li><a href="https://cursor.com/blog/warp-decode">Better MoE model inference with warp decode · Cursor</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://leimao.github.io/article/Transformer-Autoregressive-Inference-Optimization/">Transformer Autoregressive Inference Optimization</a></li>

</ul>
</details>

**Tags**: `#AI Inference`, `#Mixture-of-Experts`, `#GPU Optimization`, `#Blackwell GPU`, `#Systems Engineering`

---

<a id="item-5"></a>
## [Apple Seeks Supreme Court Review of App Store Fee Ruling, Secures Stay](https://techcrunch.com/2026/04/06/apple-epic-games-lawsuit-supreme-court-appeal-app-store-commission/) ⭐️ 8.0/10

Apple has secured a stay from an appeals court and plans to petition the U.S. Supreme Court to review a ruling that found it in contempt of court for imposing a 27% commission on purchases made through external payment systems. This decision follows the Ninth Circuit Court of Appeals upholding the contempt finding in December 2025 and denying Apple's request for a rehearing in March 2026. This move could lead to a landmark Supreme Court decision that redefines platform control over pricing and commissions across the entire app economy. The outcome has the potential to significantly alter developer economics, reduce costs for consumers, and set a precedent for how digital marketplaces operate under antitrust law. The core legal issue is whether Apple's 27% fee on external payments, implemented after being ordered to allow them, constitutes a good-faith compliance or a deliberate circumvention of the court's injunction. Epic Games has immediately challenged the stay, calling Apple's Supreme Court appeal "another delay tactic" to avoid a court-imposed cap on its commissions.

telegram · zaihuapd · Apr 7, 06:15

**Background**: The legal battle stems from Epic Games' 2020 antitrust lawsuit against Apple, challenging its control over the iOS app ecosystem and its 30% commission on in-app purchases. In 2021, a district court issued an injunction requiring Apple to allow developers to link to external payment methods, but did not find it to be an illegal monopolist. Apple complied by allowing external links but imposed a 27% commission, which lower courts later found to be in contempt of the original order's intent.

<details><summary>References</summary>
<ul>
<li><a href="https://siliconcanals.com/sc-n-apples-supreme-court-bid-could-redefine-who-controls-platform-pricing-across-the-app-economy/">Apple’s Supreme Court bid could redefine who controls ...</a></li>
<li><a href="https://techcrunch.com/2025/05/02/apple-changes-us-app-store-rules-to-let-apps-redirect-users-to-their-own-websites-for-payments/">Apple changes US App Store rules to let apps link to external ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Epic_Games_v._Apple">Epic Games v. Apple - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#antitrust`, `#app-store`, `#legal`, `#platform-regulation`, `#epic-games`

---

<a id="item-6"></a>
## [GitHub Issue Reports 67% Drop in Claude Code Thinking Depth, Team Attributes to Parameter Tuning](https://github.com/anthropics/claude-code/issues/42796) ⭐️ 8.0/10

A GitHub issue analyzing 6,852 Claude Code session logs from late January to early April 2026 reported a 67% reduction in the model's 'thinking depth,' from about 2,200 characters to around 720 characters, leading to degraded performance on complex engineering tasks. The Claude Code team responded that changes were due to the introduction of 'adaptive thinking' on February 9 and a default switch to 'Medium effort' on March 3, not the 'redact-thinking' UI feature. This matters because Claude Code is a major AI coding assistant, and a perceived 67% drop in reasoning depth directly impacts developers' productivity and trust in the tool for complex tasks. The team's explanation highlights the ongoing trade-offs and tuning decisions AI providers make between computational cost, response speed, and output quality, which can significantly affect user experience. The analysis was based on a substantial dataset of 6,852 real user sessions, indicating a data-driven community concern. The team clarified that the 'redact-thinking' feature only hides the thinking text in the UI for all users but does not affect the underlying model reasoning, and users can adjust or turn off the 'Medium effort' default in settings.

telegram · zaihuapd · Apr 7, 07:43

**Background**: Claude Code is a terminal-based AI coding assistant that can show its internal 'thinking' process before delivering a final answer, which is believed to correlate with reasoning depth and problem-solving quality. 'Effort levels' (like Low, Medium, High) are configurable parameters in Claude Code that control how much computational 'thinking' the model dedicates to a task, balancing speed and depth. Model providers like Anthropic frequently adjust these parameters server-side to optimize performance and cost, which can lead to noticeable changes in user-observed behavior without a client-side update.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/how-claude-code-works">How Claude Code works - Claude Code Docs</a></li>
<li><a href="https://llmx.tech/blog/how-to-change-claude-code-effort-level-best-settings-per-subscription-tier/">How to Change Claude Code Effort Level: Best Settings Per ...</a></li>
<li><a href="https://code.claude.com/docs/en/model-config">Model configuration - Claude Code Docs</a></li>

</ul>
</details>

**Tags**: `#AI-Coding-Assistants`, `#Claude`, `#Model-Performance`, `#GitHub-Discussions`, `#LLM-Tuning`

---

<a id="item-7"></a>
## [Artemis II Crew Breaks 54-Year-Old Record for Farthest Human Spaceflight from Earth](https://www.nasa.gov/news-release/nasas-artemis-ii-crew-eclipses-record-for-farthest-human-spaceflight/) ⭐️ 8.0/10

On April 6, 2026, at 1:56 p.m. EDT, the four astronauts of NASA's Artemis II mission reached a distance of 248,655 miles from Earth, surpassing the record set by Apollo 13 in 1970. The crew is expected to reach their maximum planned distance of approximately 252,756 miles from Earth during their lunar flyby. This milestone marks the first time in over half a century that humans have traveled this far into space, signaling a major step forward in NASA's Artemis program to return humans to the Moon and eventually explore Mars. Breaking a record held since the Apollo era demonstrates tangible progress in modern deep-space exploration capabilities and rekindles public interest in crewed lunar missions. The mission, launched on April 1 from Kennedy Space Center, is past its halfway point and will make its closest approach to the lunar surface at about 4,067 miles. During this flyby, the spacecraft will experience a communications blackout of about 40 minutes due to the Moon blocking the signal with Earth, and is scheduled to splash down in the Pacific Ocean off San Diego on April 11.

telegram · zaihuapd · Apr 7, 08:31

**Background**: Artemis II is the first crewed mission of NASA's Artemis program and the first crewed flight of the Orion spacecraft. Its primary objective is to test and validate the spacecraft's systems with a crew onboard during a lunar flyby, paving the way for future lunar landings. The previous record was held by the Apollo 13 mission in April 1970, which reached an altitude of approximately 248,573 miles from Earth during its emergency free-return trajectory around the Moon.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Artemis_II">Artemis II - Wikipedia</a></li>
<li><a href="https://www.nasa.gov/mission/artemis-ii/">Artemis II : NASA’s First Crewed Lunar Flyby in 50 Years - NASA</a></li>
<li><a href="https://www.cnbc.com/2026/04/06/artemis-ii-breaks-apollo-13s-distance-record.html">Artemis II breaks Apollo 13’s distance record - CNBC Artemis II breaks Apollo 13 record, now farthest distance in ... Artemis II crew breaks Apollo 13 record, reaching 252,760 ... Artemis II breaks NASA Apollo 13 space distance record during ... Highest altitude reached by humans - Guinness World Records</a></li>

</ul>
</details>

**Tags**: `#space-exploration`, `#nasa`, `#artemis-program`, `#human-spaceflight`, `#lunar-mission`

---

<a id="item-8"></a>
## [Tesla officially adapts its app for Huawei's HarmonyOS, becoming the first major overseas automaker to join the ecosystem.](https://finance.sina.com.cn/tech/mobile/n/n/2026-04-07/doc-inhtsezc7200912.shtml) ⭐️ 8.0/10

Tesla's official app has recently been launched on Huawei's AppGallery, supporting remote vehicle control, phone-as-key functionality, media control, temperature adjustment, service scheduling, charging management, and roadside assistance requests. This makes Tesla the first major overseas automaker to officially adapt its application for Huawei's HarmonyOS. This move signifies a strategic endorsement of HarmonyOS's commercial value and device scale by a leading global manufacturer, potentially accelerating the operating system's international expansion beyond China. It represents a notable development in cross-platform integration within the automotive-tech space and could influence other international brands to consider HarmonyOS compatibility. The adaptation involves publishing the Tesla app on Huawei's AppGallery, allowing HarmonyOS users direct access. It leverages Tesla's existing APIs for vehicle data and control, which are also available to third-party developers, but this represents an official, first-party integration with Huawei's platform.

telegram · zaihuapd · Apr 7, 09:00

**Background**: HarmonyOS is a distributed operating system developed by Huawei for a wide range of smart devices, including smartphones, tablets, and wearables. It is positioned as an alternative to Android and iOS, with Huawei actively building its independent ecosystem. Tesla provides a set of APIs that allow third-party developers to build applications that interact with Tesla vehicles for functions like remote control and data access.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HarmonyOS">HarmonyOS - Wikipedia</a></li>
<li><a href="https://www.tesla.com/developer-docs">Getting Started With Third-Party Apps | Tesla</a></li>

</ul>
</details>

**Tags**: `#automotive-software`, `#harmonyos`, `#tesla`, `#mobile-ecosystems`, `#tech-partnerships`

---

<a id="item-9"></a>
## [New Yorker Investigation Alleges Pattern of Deception by OpenAI CEO Sam Altman](https://www.newyorker.com/magazine/2026/04/13/sam-altman-may-control-our-future-can-he-be-trusted) ⭐️ 8.0/10

The New Yorker published a major investigation alleging that OpenAI CEO Sam Altman has engaged in a long-term pattern of deception and power manipulation, based on internal documents including a secret memo from Ilya Sutskever and over 200 pages of private notes from Dario Amodei, plus interviews with over 100 sources. The report details how Altman was fired by the board in late 2023 for being "not consistently candid," only to be reinstated days later after a major employee revolt, leading to a board overhaul. This matters because it raises profound questions about the trustworthiness and governance of a company at the forefront of developing artificial general intelligence (AGI), a technology with potentially civilization-altering consequences. The allegations suggest that OpenAI's leadership may have misled its board, the public, and regulators about safety commitments and internal practices, which could undermine public trust in AI development and have significant implications for AI safety and corporate governance globally. Key allegations include Altman reportedly promising to dedicate 20% of computing power to safety research but only allocating 1-2%, leading to the team's eventual dissolution, and concealing from the board that GPT-4's capabilities were deployed without full approval. After his reinstatement, an agreed-upon external 'review' resulted only in an oral briefing to two new board members, with no written report, minimizing the formal record of the allegations.

telegram · zaihuapd · Apr 7, 14:07

**Background**: OpenAI was founded in 2015 as a non-profit research lab with a mission to ensure that artificial general intelligence (AGI) benefits all of humanity. Its unique capped-profit structure was designed to prioritize this mission over shareholder returns. In November 2023, the company's board of directors, which originally included members associated with the 'effective altruism' movement focused on long-term existential risks, abruptly fired CEO Sam Altman, citing a lack of candor, but he was reinstated within days after most employees threatened to quit.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@prateekj24/the-52-page-memo-that-nearly-destroyed-openai-inside-ilya-sutskevers-deposition-acef91208a1c">The 52-Page Memo That Nearly Destroyed OpenAI: Inside Ilya ...</a></li>
<li><a href="https://forum.effectivealtruism.org/topics/ai-governance">AI governance - EA Forum - Effective altruism</a></li>

</ul>
</details>

**Tags**: `#AI Ethics`, `#Corporate Governance`, `#OpenAI`, `#Leadership`, `#Investigative Journalism`

---

<a id="item-10"></a>
## [Telegram Enables Direct Bot-to-Bot Communication for AI Agent Collaboration](https://core.telegram.org/bots/features) ⭐️ 7.0/10

Telegram has officially launched bot-to-bot communication, allowing different bots to interact directly within groups or through business account interfaces. Developers can enable this feature via @BotFather, enabling bots to respond to mentions or replies from other bots, facilitating complex automated workflows. This represents a significant expansion of Telegram's bot ecosystem, moving beyond simple human-to-bot interactions to enable multi-agent AI systems that can collaborate on complex tasks. It positions Telegram as a platform for sophisticated automation, potentially transforming customer service, scheduling, and workflow management for businesses and developers. The feature requires explicit activation by developers through @BotFather, and interactions can occur either in groups (via mentions or replies) or within business account contexts where bots can call each other as tools. This enables specialized bots to handle different parts of a workflow, such as one managing appointments while another processes customer inquiries.

telegram · zaihuapd · Apr 7, 06:54

**Background**: Telegram bots are automated accounts that users can interact with through messages and commands, commonly used for customer support, notifications, and simple tasks. AI agents are autonomous digital workers that can execute tasks, make decisions, and integrate into workflows, with multi-agent collaboration referring to multiple specialized agents working together to solve complex problems. Previously, Telegram bots primarily responded to human users, limiting their ability to coordinate with each other for advanced automation.

<details><summary>References</summary>
<ul>
<li><a href="https://clickup.com/blog/ai-multi-agent-workflow/">AI Multi-Agent Workflows: How They Work + Real Examples</a></li>
<li><a href="https://www.taskade.com/blog/what-are-ai-agents">What Are AI Agents? The Future Of Workflow Automation ...</a></li>

</ul>
</details>

**Tags**: `#telegram`, `#chatbots`, `#automation`, `#ai-agents`, `#messaging-platforms`

---