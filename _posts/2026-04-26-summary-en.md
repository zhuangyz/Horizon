---
layout: default
title: "Horizon Summary: 2026-04-26 (EN)"
date: 2026-04-26
lang: en
---

> From 19 items, 10 important content pieces were selected

---

1. [DeepSeek-V4 Preview Released and Open-Sourced](#item-1) ⭐️ 9.0/10
2. [Asahi Linux Progress Report 7.0: M3 Hardware Enablement Advances](#item-2) ⭐️ 8.0/10
3. [Amateur uses ChatGPT to solve 60-year-old Erdős problem](#item-3) ⭐️ 8.0/10
4. [Why Alzheimer's Research Has Stalled: The Amyloid Trap](#item-4) ⭐️ 8.0/10
5. [West's loss of coding skills mirrors manufacturing decline](#item-5) ⭐️ 8.0/10
6. [OpenAI Launches GPT-5.5 Biosafety Bug Bounty Program](#item-6) ⭐️ 8.0/10
7. [1900 US Academy Members Urge Trump to Stop Attacks on Science](#item-7) ⭐️ 8.0/10
8. [Top university websites hijacked to serve porn due to DNS neglect](#item-8) ⭐️ 8.0/10
9. [Headspace App Silently Installs on iPhones Daily](#item-9) ⭐️ 7.0/10
10. [Chinese GPU Maker Licuan 7G100 Gets WHQL Certification](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [DeepSeek-V4 Preview Released and Open-Sourced](https://t.me/zaihuapd/41074) ⭐️ 9.0/10

DeepSeek has released the preview version of DeepSeek-V4, including V4-Pro and V4-Flash variants, and open-sourced the model weights. The V4-Pro model surpasses all current open-source models in math, STEM, and competitive coding benchmarks, approaching the performance of the top three proprietary models. This release represents a major milestone in open-weight large language models, potentially reshaping the competitive landscape by offering state-of-the-art performance at a much lower cost. The dramatically improved Agent capabilities make it highly suitable for real-world automation and tool-use tasks, benefiting developers and enterprises. DeepSeek-V4-Pro is a Mixture-of-Experts (MoE) model with 1.6 trillion total parameters and 49 billion active parameters, featuring a 1-million-token context window. The V4-Flash variant offers faster and more economical API service with smaller parameter activation, while still delivering strong reasoning and Agent capabilities.

telegram · zaihuapd · Apr 26, 07:17

**Background**: DeepSeek is a Chinese AI company known for developing high-performance open-source language models. The term 'Agent' refers to the model's ability to autonomously use tools, call functions, and execute multi-step tasks, which is critical for practical applications like coding assistants and automated workflows. The '御三家' (top three) refers to leading proprietary models such as GPT-4o and Claude Opus.

<details><summary>References</summary>
<ul>
<li><a href="https://www.knightli.com/en/2026/04/24/deepseek-v4-preview-release/">DeepSeek-V4 Preview Released: 1M Context, Two Models, and API ...</a></li>
<li><a href="https://stable-learn.com/en/deepseek-v4-release/">DeepSeek-V4: 1M Context, Best Open-Source Agent, Beats Claude ...</a></li>
<li><a href="https://deepinfra.com/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/ DeepSeek - V 4 -Pro - Demo - DeepInfra</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#LLM`, `#open-source`, `#AI`, `#Agent`

---

<a id="item-2"></a>
## [Asahi Linux Progress Report 7.0: M3 Hardware Enablement Advances](https://asahilinux.org/2026/04/progress-report-7-0/) ⭐️ 8.0/10

Asahi Linux's progress report 7.0 announces that patches for M3 Macs have been added to the Asahi kernel tree, enabling PCIe, NVMe, keyboard/trackpad, SMC-based RTC, and reboot controller support, bringing M3 support to roughly the same level as the first M1 alpha. This milestone significantly expands Linux compatibility to Apple's latest M3 hardware, offering users a viable alternative to macOS on high-performance Apple Silicon Macs and demonstrating the project's sustained reverse-engineering success. The enablement work was contributed by Michael Reeves and Alyssa Milburn, and the audio driver for the CS42L84 codec currently only supports 48 kHz and 96 kHz sample rates, as those are the only rates programmed by macOS.

hackernews · elisaado · Apr 26, 10:50

**Background**: Asahi Linux is a community-driven project that ports Linux to Apple Silicon Macs by reverse-engineering undocumented hardware. Apple's M1, M2, M3, and newer chips use a custom ARM-based architecture that lacks official public documentation, making driver development exceptionally challenging. The project released its first alpha for M1 in March 2022, and progress on M3 now mirrors that early milestone.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asahi_linux_project">Asahi linux project</a></li>
<li><a href="https://en.wikipedia.org/wiki/Asahi_Linux">Asahi Linux - Wikipedia</a></li>
<li><a href="https://asahilinux.org/">Asahi Linux</a></li>

</ul>
</details>

**Discussion**: The community expressed enthusiasm for M3 progress, with some users praising the technical write-ups and hoping the project gains momentum. However, skepticism remains about long-term sustainability, as the effort is still separate from mainline kernel and mainstream distributions, and some questioned why Apple does not provide official documentation to aid the project.

**Tags**: `#Asahi Linux`, `#Apple Silicon`, `#Linux kernel`, `#reverse engineering`, `#M3`

---

<a id="item-3"></a>
## [Amateur uses ChatGPT to solve 60-year-old Erdős problem](https://www.scientificamerican.com/article/amateur-armed-with-chatgpt-vibe-maths-a-60-year-old-problem/) ⭐️ 8.0/10

An amateur mathematician used ChatGPT to generate a novel approach that helped solve a 60-year-old Erdős problem, with the raw output later refined by experts including mathematician Jared Lichtman and Terence Tao. This demonstrates that large language models can contribute creative insights to long-standing open problems in mathematics, potentially accelerating research by breaking through human mental blocks. The raw ChatGPT proof was poor and required expert curation, but it contained a key insight that led to a shortened, rigorous proof. The problem was perhaps easier than previously thought, suggesting AI can help clear the deck of such problems.

hackernews · pr337h4m · Apr 25, 17:40

**Background**: Paul Erdős was a prolific Hungarian mathematician known for posing many unsolved problems, often with monetary rewards. Erdős problems range widely in difficulty and have challenged mathematicians for decades. This particular problem had remained unsolved for about 60 years.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Erdős_problem">Erdős problem</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_conjectures_by_Paul_Erdős">List of conjectures by Paul Erdős - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments highlight that the raw ChatGPT output was poor but its key insight was valuable, and that the problem may have been easier than expected, with AI helping to overcome mental blocks. Some note that the headline oversimplifies the collaborative effort required.

**Tags**: `#AI`, `#mathematics`, `#LLM`, `#research`, `#Erdős problem`

---

<a id="item-4"></a>
## [Why Alzheimer's Research Has Stalled: The Amyloid Trap](https://freakonomics.com/podcast/why-has-there-been-so-little-progress-on-alzheimers-disease/) ⭐️ 8.0/10

A Freakonomics podcast examines why decades of Alzheimer's research have yielded little progress, focusing on the failure of the amyloid hypothesis and the scientific community's resistance to alternative approaches. This matters because Alzheimer's affects millions worldwide, and the stagnation in research has wasted billions in funding and delayed potential treatments, highlighting systemic problems in how medical science pursues dominant paradigms. The podcast and community comments point to the amyloid cascade hypothesis—the idea that amyloid-beta plaques cause Alzheimer's—as a dominant but flawed model that has locked in funding and research for decades, while alternative theories like tau pathology, inflammation, and senescence were sidelined.

hackernews · chiefalchemist · Apr 26, 00:12

**Background**: The amyloid cascade hypothesis, proposed in the 1990s, posits that accumulation of amyloid-beta peptides in the brain triggers a cascade leading to Alzheimer's disease. This hypothesis has guided most drug development efforts for over two decades, but clinical trials targeting amyloid have repeatedly failed to show meaningful cognitive benefits in patients.

<details><summary>References</summary>
<ul>
<li><a href="https://academic.oup.com/brain/article/146/10/3969/7162122">The amyloid cascade hypothesis: an updated critical review</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9662281/">Amyloid Cascade Hypothesis for the Treatment of Alzheimer’s ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Paradigm_shift">Paradigm shift - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that the amyloid hypothesis was a costly mistake, with some attributing it to scientific inertia and funding lock-in rather than malice. One user recommends Karl Herrup's book 'How Not to Study a Disease' as a key critique, while another argues that Alzheimer's is a product of senescence, a root cause the medical system avoids addressing.

**Tags**: `#Alzheimer's`, `#medical research`, `#scientific paradigm`, `#pharmaceutical industry`, `#public health`

---

<a id="item-5"></a>
## [West's loss of coding skills mirrors manufacturing decline](https://techtrenches.dev/p/the-west-forgot-how-to-make-things) ⭐️ 8.0/10

An article argues that the West's historical loss of manufacturing expertise is now being replicated in software engineering, as reliance on AI and short-term cost-cutting erodes deep coding knowledge and mentorship. This trend threatens the long-term health of the software industry by weakening the transfer of tacit knowledge, which is critical for innovation and problem-solving, and could lead to a generation of developers overly dependent on AI tools. The article highlights that short-term cost-cutting reduces junior hiring and removes the organizational slack needed for experienced engineers to teach, causing tacit knowledge to stop being transferred and leaving only documentation and automation.

hackernews · milkglass · Apr 26, 06:24

**Background**: Tacit knowledge is the unwritten, intuitive understanding gained through hands-on experience and mentorship, which is difficult to capture in documentation or code. The West's earlier decline in manufacturing skills is often attributed to offshoring and a focus on short-term profits, a pattern the article argues is now repeating in software development.

**Discussion**: Community comments largely agree with the article's premise, with one user blaming management patterns that prioritize short-term cost-cutting over knowledge transfer, while another notes that relying on AI for trivial tasks is 'scary' because it means brain skills atrophy. A third commenter criticizes the article itself as AI-generated, pointing out that writing ability is also a skill that atrophies.

**Tags**: `#software engineering`, `#AI`, `#knowledge transfer`, `#management`, `#skill atrophy`

---

<a id="item-6"></a>
## [OpenAI Launches GPT-5.5 Biosafety Bug Bounty Program](https://openai.com/zh-Hans-CN/index/gpt-5-5-bio-bug-bounty/) ⭐️ 8.0/10

OpenAI has launched a biosafety bug bounty program for GPT-5.5, offering a $25,000 reward for the first universal jailbreak prompt that bypasses all five biosafety challenges without triggering content moderation. The program is invitation-only, with applications open from April 23 to June 22, 2026, and testing from April 28 to July 27, 2026. This program represents a significant investment in proactive AI safety research, specifically targeting the risk of AI being misused to generate dangerous biological information. By incentivizing external red-teamers to find universal jailbreaks, OpenAI aims to strengthen GPT-5.5's guardrails before broader deployment, setting a precedent for responsible AI development in high-risk domains. The testing scope is limited to GPT-5.5 within Codex Desktop only, and participants must sign a non-disclosure agreement. The challenge requires a single universal jailbreak prompt that successfully answers all five biosafety questions from a clean chat without triggering the model's moderation system.

telegram · zaihuapd · Apr 25, 16:36

**Background**: A universal jailbreak is a single prompt that can bypass an AI model's safety guardrails across multiple tasks, rather than exploiting a specific vulnerability. Biosafety in AI refers to the risk that advanced language models could provide detailed instructions for creating biological threats, such as pathogens or toxins. OpenAI has been iterating on GPT-5.x models, with GPT-5.4 released in March 2026, and GPT-5.5 now available in Codex Desktop for ChatGPT users.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-5-bio-bug-bounty/">GPT‑5.5 Bio Bug Bounty - OpenAI</a></li>
<li><a href="https://openai.smapply.org/prog/gpt-5-5-safety-bio-bounty-program">GPT-5.5 Bio Bounty Program - OpenAI</a></li>
<li><a href="https://gbhackers.com/gpt-5-5-bio-bug-bounty-program/">GPT-5.5 Bio Bug Bounty Program Aims to Improve AI Safety and ...</a></li>

</ul>
</details>

**Tags**: `#AI Safety`, `#Bug Bounty`, `#GPT-5.5`, `#Biosafety`, `#OpenAI`

---

<a id="item-7"></a>
## [1900 US Academy Members Urge Trump to Stop Attacks on Science](https://t.me/zaihuapd/41070) ⭐️ 8.0/10

On March 31, 1900 members of the US National Academies of Sciences, Engineering, and Medicine, including over a dozen Nobel laureates, published an open letter calling on the Trump administration to halt what they describe as a comprehensive assault on American science. This unprecedented mobilization of top scientists signals a major policy conflict that could disrupt research funding, weaken public trust in science, and harm US global leadership in innovation and health. The letter was drafted by 13 scientists from fields including medicine, epidemiology, psychology, climate science, sociology, and economics, and signatories include Nobel laureates such as Harvey J. Alter, Francoise Barre-Sinoussi, Reinhard Genzel, Edvard I. Moser, and May-Britt Moser.

telegram · zaihuapd · Apr 26, 00:40

**Background**: The US National Academies are prestigious honorary societies that advise the government on science and technology. The Trump administration has proposed significant budget cuts to agencies like the NIH and NSF, and has taken actions that scientists view as undermining evidence-based policy, such as withdrawing from the Paris Agreement and downplaying climate change.

**Tags**: `#science policy`, `#research funding`, `#Trump administration`, `#open letter`, `#US academia`

---

<a id="item-8"></a>
## [Top university websites hijacked to serve porn due to DNS neglect](https://arstechnica.com/security/2026/04/why-are-top-university-websites-serving-porn-it-comes-down-to-shoddy-housekeeping/) ⭐️ 8.0/10

At least 34 top universities, including UC Berkeley and Columbia, have had their subdomains hijacked by the Hazy Hawk threat group to serve pornographic content and scams, exploiting unremoved CNAME records after subdomains were decommissioned. This incident highlights a widespread and critical domain management vulnerability that affects even highly reputable institutions, allowing attackers to leverage the universities' trusted domains to rank highly in search results and deceive users, potentially damaging institutional credibility and user trust. The Hazy Hawk group has been exploiting abandoned cloud resources since at least December 2023, targeting organizations like Deloitte and Panasonic, and has now compromised hundreds of university subdomains, resulting in thousands of malicious pages indexed by search engines.

telegram · zaihuapd · Apr 26, 09:02

**Background**: A CNAME record in DNS maps one domain name to another, often used to point a subdomain to an external service like a cloud platform. When a subdomain is decommissioned but its CNAME record is not removed, the record becomes a 'dangling' or orphaned DNS entry. Attackers can then register the external service endpoint referenced by the dangling record, effectively taking control of the subdomain to host malicious content.

<details><summary>References</summary>
<ul>
<li><a href="https://www.spamhaus.org/resource-hub/dns/dangling-dns-and-the-dangers-of-subdomain-hijacking/">Blog | Dangling DNS and the dangers of subdomain hijacking | Resources</a></li>
<li><a href="https://quorumcyber.com/threat-intelligence/hazy-hawk-exploits-dns-vulnerabilities-to-target-major-organisations/">Hazy Hawk Exploits DNS Vulnerabilities | Quorum Cyber</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/security/fundamentals/subdomain-takeover">Prevent dangling DNS entries and avoid subdomain takeover</a></li>

</ul>
</details>

**Tags**: `#security`, `#domain hijacking`, `#DNS`, `#cyber attack`, `#university`

---

<a id="item-9"></a>
## [Headspace App Silently Installs on iPhones Daily](https://news.ycombinator.com/item?id=47906253) ⭐️ 7.0/10

Users report that the Headspace meditation app silently installs itself on their iPhones every day around 1pm EST, despite automatic downloads being turned off and iOS being up to date. This unexplained behavior raises privacy and security concerns, as it suggests a potential iOS bug or unauthorized app installation mechanism that could affect many users beyond just Headspace. The issue has been reported on iPhone 12, 13 Pro, and even iPhone 17 Pro models, across different iOS versions and without MDM profiles, indicating it is not device-specific or MDM-related.

hackernews · _-x-_ · Apr 26, 00:50

**Background**: MDM (Mobile Device Management) profiles allow organizations to remotely install and manage apps on devices, but users in this case report no such profiles installed. A similar iOS bug in 2017 caused apps with local time-based notifications to trigger endless crash loops, and some community members draw parallels to the current issue.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=47906253">Tell HN: An app is silently installing itself on my iPhone every day</a></li>

</ul>
</details>

**Discussion**: Community members hypothesize that notification-triggered app launches combined with iOS's offloading feature could cause the app to reappear. Others recall a 2017 iOS bug involving meditation apps and local notifications, suggesting a possible recurring pattern.

**Tags**: `#iOS`, `#bug`, `#privacy`, `#app installation`, `#security`

---

<a id="item-10"></a>
## [Chinese GPU Maker Licuan 7G100 Gets WHQL Certification](http://www.cnbeta.com.tw/articles/tech/1559976.htm) ⭐️ 7.0/10

Licuan Technology's 7G100 series GPU has received Microsoft WHQL certification, making it the first Chinese and the fourth global GPU company to achieve this milestone. In benchmarks, the Lisuan eXtreme series scored 2268 in 3DMark Steel Nomad, approaching the performance of NVIDIA's RTX 4060. This certification signals that Licuan's GPU drivers meet Microsoft's rigorous quality standards, enabling broad Windows compatibility and boosting confidence in Chinese-made GPUs. It also demonstrates that domestic GPUs can compete with mainstream products like the RTX 4060 in real-world gaming and AI workloads. The 7G100 series is built on a 6nm process with Licuan's self-developed 'Tiantu' architecture, featuring fully independent design of compute cores, instruction set, and software stack. In 1080P high settings, it runs Black Myth: Wukong at over 70 FPS and supports mainstream large AI models on AIPC.

telegram · zaihuapd · Apr 26, 02:59

**Background**: WHQL (Windows Hardware Quality Labs) certification is Microsoft's testing process for third-party device drivers, ensuring stability and compatibility with Windows. Only three other GPU companies—NVIDIA, AMD, and Intel—have previously achieved this certification. Licuan's 7G100 series targets the mid-range graphics market, competing with products like the RTX 4060.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WHQL_Testing">WHQL Testing - Wikipedia</a></li>
<li><a href="https://store.steampowered.com/app/2695340/3DMark_Steel_Nomad/">3DMark Steel Nomad on Steam</a></li>

</ul>
</details>

**Tags**: `#GPU`, `#WHQL`, `#Chinese semiconductor`, `#hardware`, `#graphics`

---