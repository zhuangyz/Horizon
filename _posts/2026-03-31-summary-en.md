---
layout: default
title: "Horizon Summary: 2026-03-31 (EN)"
date: 2026-03-31
lang: en
---

> From 24 items, 7 important content pieces were selected

---

1. [Axios npm package compromised, malicious versions deliver remote access trojan](#item-1) ⭐️ 9.0/10
2. [Google Quantum AI reduces Bitcoin attack requirements 20x, potentially enabling private key extraction in under 9 minutes](#item-2) ⭐️ 9.0/10
3. [Ollama adds MLX-powered inference for Apple Silicon in preview](#item-3) ⭐️ 8.0/10
4. [Artemis II Mission Faces Critical Heat Shield Safety Concerns](#item-4) ⭐️ 8.0/10
5. [Claude Code's source code leaked via NPM source map, exposing anti-distillation defenses and roadmap.](#item-5) ⭐️ 8.0/10
6. [Unofficial GitHub Repository Reconstructs Claude Code Source from Public npm Package Source Maps](#item-6) ⭐️ 8.0/10
7. [Micron Bets on Stacked GDDR, Targets 2027 for First Samples](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Axios npm package compromised, malicious versions deliver remote access trojan](https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan) ⭐️ 9.0/10

On March 31, 2026, an attacker compromised an Axios maintainer's npm account and published two malicious versions (v1.14.1 and v0.30.4). These versions injected a fake dependency, `plain-crypto-js@4.2.1`, which executed a postinstall script to deploy a cross-platform remote access trojan (RAT). This incident is a critical supply chain attack affecting Axios, one of the most popular HTTP client libraries in the JavaScript ecosystem with over 50 million weekly downloads. The compromise could lead to immediate credential theft and persistent remote access for attackers on any system where the malicious package was installed, impacting countless downstream applications and services. The malicious code was not placed directly in the Axios source but hidden within the `plain-crypto-js` dependency's postinstall script. The attack leveraged a previously compromised maintainer account, and the malicious packages were published in quick succession early on March 31, 2026 (UTC).

hackernews · mtud · Mar 31, 02:54

**Background**: npm (Node Package Manager) is the default package registry for the JavaScript/Node.js ecosystem, hosting millions of reusable code libraries. A supply chain attack in this context involves compromising a trusted package to inject malware, which then spreads to all applications that depend on it. Remote Access Trojans (RATs) are malware that provide an attacker with control over an infected system. The `postinstall` script is a lifecycle hook in npm that runs automatically after a package is installed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wiz.io/blog/axios-npm-compromised-in-supply-chain-attack">Axios NPM Distribution Compromised in Supply Chain Attack | Wiz Blog</a></li>
<li><a href="https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan">axios Compromised on npm - Malicious Versions Drop Remote Access Trojan - StepSecurity</a></li>
<li><a href="https://www.sans.org/blog/axios-npm-supply-chain-compromise-malicious-packages-remote-access-trojan">Axios NPM Supply Chain Compromise: Malicious Packages Deliver Remote Access Trojan | SANS Institute</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights immediate mitigation strategies, such as setting a minimum package release age (e.g., 7 days) and disabling script execution via `ignore-scripts=true` in npm config, which would have prevented this attack. There is concern about the massive scale of impact due to Axios's ubiquity, and observations about a recurring attack pattern where stolen credentials are used to compromise further packages. Some commenters advocate for "batteries included" ecosystems to reduce critical third-party dependencies.

**Tags**: `#security`, `#npm`, `#supply-chain`, `#javascript`, `#malware`

---

<a id="item-2"></a>
## [Google Quantum AI reduces Bitcoin attack requirements 20x, potentially enabling private key extraction in under 9 minutes](https://research.google/blog/safeguarding-cryptocurrency-by-disclosing-quantum-vulnerabilities-responsibly/) ⭐️ 9.0/10

Google's Quantum AI team published a whitepaper demonstrating a 20x reduction in quantum computing resources needed to break Bitcoin's elliptic curve cryptography using optimized Shor's algorithm circuits. Their attack circuits require fewer than 1,200-1,450 logical qubits (built from under 500,000 physical qubits), potentially enabling private key extraction within approximately 9 minutes after a transaction is broadcast. This represents a paradigm shift in quantum vulnerability assessment, showing that practical attacks on cryptocurrency wallets could become feasible with far fewer quantum resources than previously estimated. Approximately 6.9 million Bitcoin (about one-third of the supply) are potentially at risk because their public keys are already exposed on the blockchain, with the 2021 Taproot upgrade potentially expanding this vulnerable pool. The team compiled two attack circuits requiring fewer than 1,200 and 1,450 logical qubits respectively, which could run on superconducting quantum computers with under 500,000 physical qubits. An attacker could perform most preparatory computations in advance, then extract the private key within about 9 minutes after transaction broadcast, giving them a 41% probability of stealing funds before transaction confirmation (given Bitcoin's ~10-minute block time).

telegram · zaihuapd · Mar 31, 08:03

**Background**: Bitcoin and Ethereum currently rely on Elliptic Curve Cryptography (ECC), specifically the Elliptic Curve Digital Signature Algorithm (ECDSA), for securing wallets and transactions. Shor's algorithm is a quantum computing algorithm that can efficiently solve the mathematical problems underlying ECC (and RSA), potentially allowing a quantum computer to derive a private key from a public key. Logical qubits are error-corrected computational units built from many fragile physical qubits, with quantum error correction being essential for performing reliable, complex computations like running Shor's algorithm.

<details><summary>References</summary>
<ul>
<li><a href="https://quantumai.google/static/site-assets/downloads/cryptocurrency-whitepaper.pdf">Securing Elliptic Curve Cryptocurrencies against Quantum ...</a></li>
<li><a href="https://www.coindesk.com/tech/2026/03/31/bitcoin-bulls-scramble-for-post-quantum-protection-as-google-drops-bombshell-paper">Bitcoin bulls scramble for post-quantum protection as Google ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Physical_and_logical_qubits">Physical and logical qubits - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#quantum-computing`, `#cryptocurrency-security`, `#cryptography`, `#quantum-cryptanalysis`, `#blockchain`

---

<a id="item-3"></a>
## [Ollama adds MLX-powered inference for Apple Silicon in preview](https://ollama.com/blog/mlx) ⭐️ 8.0/10

Ollama has announced preview support for MLX-powered inference on Apple Silicon devices, enabling faster and more efficient local execution of large language models (LLMs). This integration leverages Apple's MLX array framework specifically designed for machine learning on Apple silicon. This integration significantly boosts the performance and energy efficiency of running LLMs locally on Macs, making on-device AI more practical for developers and users. It strengthens the ecosystem for private, cost-effective AI applications that don't rely on cloud services or internet connectivity. The performance improvement is particularly notable on newer chips like the M5, as indicated by benchmark graphs. This feature is currently in preview, meaning it's an early release for testing and feedback before a stable version.

hackernews · redundantly · Mar 31, 03:40

**Background**: Ollama is a popular open-source tool that simplifies running open-weights large language models (LLMs) locally on a user's computer. MLX is an array framework for machine learning created by Apple and optimized for its Apple silicon chips (M1, M2, M3, M4, M5), enabling efficient computation on the GPU and Neural Engine. Running models locally with tools like Ollama offers benefits like data privacy, no API costs, and offline operation, but has traditionally been limited by the computational power of consumer hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ml-explore/mlx">GitHub - ml-explore/mlx: MLX: An array framework for Apple silicon · GitHub</a></li>
<li><a href="https://aispaces.substack.com/p/the-ultimate-guide-to-running-llms">The Ultimate Guide to Running LLMs Locally with Ollama</a></li>
<li><a href="https://medium.com/data-science-in-your-pocket/apple-m5-chip-apple-wins-the-ultimate-ai-race-0337b97177fa">Apple M5 Chip : Apple wins the ultimate AI race - Medium</a></li>

</ul>
</details>

**Discussion**: The community strongly endorses the move towards on-device LLMs, highlighting benefits like enhanced privacy, no connectivity or token costs, and reduced electricity consumption. Comments also reveal practical considerations, such as users seeking affordable local coding rigs and praising complementary tools like OMLX for features like SSD KV caching that improve workflow. There's a shared belief that local inference is the future, with performance being the key remaining hurdle.

**Tags**: `#ollama`, `#mlx`, `#apple-silicon`, `#local-llm`, `#inference`

---

<a id="item-4"></a>
## [Artemis II Mission Faces Critical Heat Shield Safety Concerns](https://idlewords.com/2026/03/artemis_ii_is_not_safe_to_fly.htm) ⭐️ 8.0/10

A detailed analysis argues that NASA's upcoming Artemis II crewed lunar mission has serious safety issues with its Orion spacecraft heat shield design, drawing parallels to the space shuttle Columbia and Challenger disasters. The concerns stem from observed material erosion during the uncrewed Artemis I test flight and the perceived inadequacy of subsequent fixes. This matters because Artemis II is NASA's first crewed mission to the Moon in over 50 years, and a heat shield failure during atmospheric reentry at lunar-return velocities would be catastrophic for the crew. The debate highlights a recurring tension within NASA's safety culture between engineering caution and programmatic schedule pressure, with implications for the entire Artemis program and future deep-space exploration. The heat shield uses an updated tile design of the Avcoat ablative material, but post-flight analysis of Artemis I showed unexpected, localized charring and erosion patterns. While NASA and contractor Lockheed Martin assert there is sufficient safety margin, critics like former NASA engineer and astronaut Tommaso P. Camarda argue the failure mode is not fully understood and the risk is unacceptable for a crewed flight.

hackernews · idlewords · Mar 31, 02:23

**Background**: The Orion spacecraft's heat shield is a critical component designed to protect the crew capsule from extreme temperatures (exceeding 2,760°C or 5,000°F) during high-speed reentry from the Moon. Unlike the Space Shuttle's reusable silica tile system, Orion uses a single-use ablative heat shield called Avcoat, which chars and erodes to carry heat away. The Space Shuttle program suffered two catastrophic losses (Challenger in 1986, Columbia in 2003) linked in part to failures in its thermal protection system and organizational safety culture.

<details><summary>References</summary>
<ul>
<li><a href="https://phys.org/news/2026-03-shield-safety-stakes-nasa-artemis.html">Heat shield safety concerns raise stakes for NASA's Artemis ...</a></li>
<li><a href="https://arstechnica.com/space/2026/01/nasa-chief-reviews-orion-heat-shield-expresses-full-confidence-in-it-for-artemis-ii/">Is Orion’s heat shield really safe? New NASA chief conducts ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Space_Shuttle_thermal_protection_system">Space Shuttle thermal protection system - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community discussion reflects deep concern and historical parallels. One commenter, preparing a Harvard lecture on systemic failures, added Artemis II to case studies alongside Challenger and Columbia, criticizing a persistent "broken safety culture." Others debate the risk level, with some pointing to a more balanced external article suggesting most NASA engineers and astronauts believe it is safe, while a skeptic questions why the Apollo-era heat shield design isn't being reused, hinting at possible increased mission complexity or past luck.

**Tags**: `#space-exploration`, `#safety-engineering`, `#systems-failure`, `#risk-management`, `#organizational-culture`

---

<a id="item-5"></a>
## [Claude Code's source code leaked via NPM source map, exposing anti-distillation defenses and roadmap.](https://twitter.com/Fried_rice/status/2038894956459290963) ⭐️ 8.0/10

The entire source code for Anthropic's Claude Code tool was accidentally exposed when a source map file was included in its published NPM package. This leak revealed proprietary anti-distillation defense mechanisms and details of unreleased features like an 'assistant mode' codenamed 'kairos'. This is a significant security incident that exposes proprietary AI safety techniques and product strategy, potentially undermining Anthropic's competitive advantage and security posture. It highlights a critical software supply chain vulnerability that could affect any company publishing JavaScript packages. The leak occurred because of a suspected bug in Bun (a JavaScript runtime owned by Anthropic) that caused source maps to be exposed in production builds. The exposed code includes an 'ANTI_DISTILLATION_CC' defense that injects decoy tool definitions into API requests to poison potential training data for competing models.

hackernews · treexs · Mar 31, 09:00

**Background**: Source maps are files that map minified or bundled JavaScript code back to its original source code, aiding developers in debugging. They are typically excluded from production releases. Anti-distillation is a defense technique used by AI companies to prevent competitors from extracting model capabilities by scraping API outputs for training data. Claude Code is Anthropic's AI-powered coding agent tool for developers.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/gabrielanhaia/claude-codes-entire-source-code-was-just-leaked-via-npm-source-maps-heres-whats-inside-cjo">Claude Code's Entire Source Code Was Just Leaked via npm ...</a></li>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Discussion**: The community identified a potential root cause in a Bun bug that incorrectly exposes source maps in production builds. Commenters analyzed the exposed anti-distillation defense mechanism and expressed concern over the revelation of unreleased product features, viewing it as a major strategic loss. There was also discussion about Anthropic's response, noting they deprecated rather than unpublished the vulnerable package version.

**Tags**: `#security`, `#ai-safety`, `#source-code-leak`, `#anthropic`, `#npm`

---

<a id="item-6"></a>
## [Unofficial GitHub Repository Reconstructs Claude Code Source from Public npm Package Source Maps](https://github.com/ChinaSiro/claude-code-sourcemap) ⭐️ 8.0/10

An unofficial GitHub repository named 'claude-code-sourcemap' has reconstructed 4,756 TypeScript source files of Anthropic's Claude Code version 2.1.88. This was achieved by extracting the original source code embedded within the `sourcesContent` field of the public `cli.js.map` source map file included in the `@anthropic-ai/claude-code` npm package. This incident highlights a significant security oversight where sensitive, proprietary source code was inadvertently exposed in a production build. It provides rare, detailed insight into the internal architecture of a major AI coding assistant, which could be used for security research, competitive analysis, or potentially malicious purposes. The reconstructed code includes 1,884 `.ts` and `.tsx` source files covering modules like CLI entry points, tools, commands, services, plugins, voice interaction, and Vim mode. The repository maintainer explicitly warns users not to connect Claude Code to this repository, as the remote URL hash included in the source could pose an account security risk.

telegram · zaihuapd · Mar 31, 09:33

**Background**: Source maps are files that map minified or transpiled JavaScript code back to its original source code (like TypeScript), aiding in debugging. The optional `sourcesContent` field can embed the full original source code directly within the map file. While convenient for debugging, including `sourcesContent` in publicly distributed production packages is a security risk, as it effectively publishes the original, unobfuscated source code.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.openreplay.com/source-maps-work/">What Are Source Maps and How Do They Work - blog.openreplay.com</a></li>
<li><a href="https://stackoverflow.com/questions/19802462/do-source-maps-include-the-source-text">Do source maps include the source text? - Stack Overflow</a></li>

</ul>
</details>

**Tags**: `#reverse-engineering`, `#source-code`, `#ai-tools`, `#security`, `#anthropic`

---

<a id="item-7"></a>
## [Micron Bets on Stacked GDDR, Targets 2027 for First Samples](https://www.etnews.com/20260330000228) ⭐️ 7.0/10

Micron has initiated R&D for a novel stacked GDDR memory product, with plans to complete equipment deployment and begin process testing in the second half of 2026, aiming to release a roughly 4-layer stacked sample as early as 2027. This development is significant as it aims to create a new memory tier positioned between high-cost HBM and standard GDDR, potentially offering a more cost-effective, high-bandwidth solution for AI accelerators and GPUs, thereby capturing a new market segment. The product faces significant technical challenges including chip-to-chip interconnects, power consumption, thermal management, and cost control for the stacking process. Notably, competitors Samsung and SK Hynix have not yet announced similar public plans.

telegram · zaihuapd · Mar 31, 00:36

**Background**: GDDR (Graphics Double Data Rate) and HBM (High Bandwidth Memory) are two primary high-performance memory technologies for GPUs and accelerators. Traditional GDDR uses 2D, discrete chips, while HBM employs 3D stacking with Through-Silicon Vias (TSVs) for much higher bandwidth and density, but at a significantly higher cost. Stacked GDDR is an attempt to blend the cost structure of GDDR with some of the performance benefits of 3D stacking.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1936817919486034471">GDDR 和 HBM 的对比 - 知乎</a></li>
<li><a href="https://blog.csdn.net/sinat_37574187/article/details/149797636">HBM vs GDDR有什么异同和优劣 - CSDN博客</a></li>
<li><a href="https://ee.ofweek.com/2025-03/ART-8420-2800-30658974.html">面向高性能的3D-IC芯片堆叠技术，如何普及？——技术现状、挑战与未来前...</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#memory`, `#ai-hardware`, `#gpu`, `#manufacturing`

---