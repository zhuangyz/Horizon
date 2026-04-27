---
layout: default
title: "Horizon Summary: 2026-04-27 (EN)"
date: 2026-04-27
lang: en
---

> From 12 items, 4 important content pieces were selected

---

1. [DeepSeek-V4 Preview Released and Open-Sourced with Enhanced Agent Abilities](#item-1) ⭐️ 9.0/10
2. [AI Should Elevate Thinking, Not Replace It](#item-2) ⭐️ 8.0/10
3. [Lishuan 7G100 GPU Passes Microsoft WHQL Certification](#item-3) ⭐️ 8.0/10
4. [Top University Sites Hijacked to Serve Porn Due to DNS Lapses](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DeepSeek-V4 Preview Released and Open-Sourced with Enhanced Agent Abilities](https://t.me/zaihuapd/41074) ⭐️ 9.0/10

DeepSeek has released a preview version of DeepSeek-V4, which is fully open-sourced and includes two variants: DeepSeek-V4-Pro and DeepSeek-V4-Flash. The Pro version surpasses all other open-source models in math, STEM, and competitive coding benchmarks, rivaling top closed-source models. This release marks a significant leap in open-source AI model capabilities, particularly in agent performance, making advanced AI more accessible and affordable. The combination of high performance and low cost could accelerate adoption in real-world applications like automated workflows and coding assistants. DeepSeek-V4-Pro has 1.6 trillion total parameters with 49 billion active parameters, while DeepSeek-V4-Flash has 284 billion total and 13 billion active parameters. The Flash variant offers faster and more economical API services while maintaining strong reasoning and agent capabilities.

telegram · zaihuapd · Apr 26, 07:17

**Background**: DeepSeek is a Chinese AI research company known for developing open-source large language models. Agent capabilities refer to a model's ability to autonomously use tools, execute multi-step tasks, and interact with external systems, which is crucial for building practical AI assistants. The 'three major models' (御三家) likely refers to leading closed-source models like GPT-4, Claude, and Gemini.

<details><summary>References</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/news/news260424">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>
<li><a href="https://huggingface.co/blog/deepseekv4">DeepSeek-V4: a million-token context that agents can actually use</a></li>
<li><a href="https://artificialanalysis.ai/articles/deepseek-is-back-among-the-leading-open-weights-models-with-v4-pro-and-v4-flash">DeepSeek is back among the leading open weights models with V4 Pro and V4 Flash</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#open-source`, `#AI model`, `#agent`, `#machine learning`

---

<a id="item-2"></a>
## [AI Should Elevate Thinking, Not Replace It](https://www.koshyjohn.com/blog/ai-should-elevate-your-thinking-not-replace-it/) ⭐️ 8.0/10

A widely discussed essay argues that AI should augment human judgment and reasoning rather than replace them, emphasizing that true mastery cannot be outsourced to AI tools. This argument is critical for software engineering and education, as it challenges the growing trend of relying on AI for code generation and problem-solving, warning against cognitive atrophy and loss of deep understanding. The essay specifically states that there is no shortcut to judgment, and that no generated explanation can transfer mastery into a person's brain without them doing the work themselves.

hackernews · koshyjohn · Apr 26, 20:03

**Background**: The essay is part of an ongoing debate in the software engineering community about the appropriate role of AI tools. Many engineers worry that over-reliance on AI for coding tasks may erode fundamental skills like reasoning and debugging, similar to how earlier abstractions (e.g., IDEs, package managers) changed but did not eliminate the need for understanding.

**Discussion**: Community comments show broad agreement with the essay's core point, but also add nuance: some compare AI to earlier abstractions like IDEs or package managers, arguing that the definition of 'engineer' may evolve. Others distinguish between using AI to write code one still owns versus using it as a black-box abstraction layer, with the latter seen as acceptable only for short-lived prototypes.

**Tags**: `#AI`, `#software engineering`, `#critical thinking`, `#education`, `#productivity`

---

<a id="item-3"></a>
## [Lishuan 7G100 GPU Passes Microsoft WHQL Certification](http://www.cnbeta.com.tw/articles/tech/1559976.htm) ⭐️ 8.0/10

Lishuan Technology's 7G100 series GPU has received Microsoft WHQL certification, making it the first Chinese GPU company and the fourth globally to achieve this. In benchmarks, the Lisuan eXtreme series scored 2268 in 3DMark Steel Nomad, approaching the performance of an NVIDIA RTX 4060. This certification marks a significant milestone for China's domestic GPU industry, demonstrating that a homegrown GPU can achieve Windows compatibility and competitive performance against mainstream NVIDIA cards. It could boost confidence in Chinese semiconductor alternatives for gaming and AI workloads. The 7G100 series is built on a 6nm process and Lishuan's self-developed 'Tiantu' architecture, with fully independent design of compute cores, instruction set, and software stack. In 1080P high-quality settings, it runs the game 'Black Myth: Wukong' at over 70 FPS and supports mainstream large AI models.

telegram · zaihuapd · Apr 26, 02:59

**Background**: WHQL (Windows Hardware Quality Labs) certification is Microsoft's official testing program that ensures hardware drivers are compatible and stable with Windows. It is a critical requirement for any GPU intended for the consumer Windows market. Lishuan Technology is a Chinese GPU startup founded by industry veterans with over 20 years of experience, focusing on fully self-developed GPU architectures.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lisuantech.com/">砺算科技-首页</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/2016985798424167913">砺算科技消费级LX 7G100显卡京东618首发，完全国产自主GPU架构</a></li>
<li><a href="https://learn.microsoft.com/en-us/windows-hardware/drivers/install/whql-release-signature">WHQL Release Signature - Windows drivers | Microsoft Learn</a></li>

</ul>
</details>

**Tags**: `#GPU`, `#WHQL`, `#Chinese semiconductor`, `#hardware`, `#benchmark`

---

<a id="item-4"></a>
## [Top University Sites Hijacked to Serve Porn Due to DNS Lapses](https://arstechnica.com/security/2026/04/why-are-top-university-websites-serving-porn-it-comes-down-to-shoddy-housekeeping/) ⭐️ 8.0/10

At least 34 top universities, including UC Berkeley and Columbia, had their subdomains hijacked by the threat actor Hazy Hawk to serve pornographic content and scams, exploiting CNAME records left active after subdomains were decommissioned. This incident highlights a critical domain management vulnerability that can undermine the trust in high-authority domains like .edu, as hijacked pages rank highly in search results and expose users to harmful content. Hundreds of subdomains were affected, leading to thousands of malicious pages indexed by search engines; the attack relies on administrators failing to remove CNAME records after decommissioning cloud services or subdomains.

telegram · zaihuapd · Apr 26, 09:02

**Background**: A CNAME record is a DNS entry that maps one domain to another, often used to point subdomains to cloud services. When a subdomain is decommissioned but its CNAME record remains, an attacker can register the abandoned cloud endpoint and take control of the subdomain, a technique known as subdomain takeover or dangling DNS.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/hazy-hawk-gang-exploits-dns-misconfigs-to-hijack-trusted-domains/">Hazy Hawk gang exploits DNS misconfigs to hijack trusted domains</a></li>
<li><a href="https://www.spamhaus.org/resource-hub/dns/dangling-dns-and-the-dangers-of-subdomain-hijacking/">Blog | Dangling DNS and the dangers of subdomain hijacking | Resources</a></li>
<li><a href="https://www.infoblox.com/threat-intel/threat-actors/hazy-hawk/">Hazy Hawk: Domain Hijacking Threat Actor - Infoblox</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#domain hijacking`, `#DNS`, `#university`, `#vulnerability`

---