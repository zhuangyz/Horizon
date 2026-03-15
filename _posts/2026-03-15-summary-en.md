---
layout: default
title: "Horizon Summary: 2026-03-15 (EN)"
date: 2026-03-15
lang: en
---

> From 20 items, 6 important content pieces were selected

---

1. [Scientists achieve vitrification and functional recovery of adult mouse brain tissue](#item-1) ⭐️ 9.0/10
2. [Jazzband Python Project Shuts Down Due to AI-Generated Spam PRs](#item-2) ⭐️ 8.0/10
3. [Glassworm Attack Uses Invisible Unicode Characters to Compromise Over 151 GitHub Repos](#item-3) ⭐️ 8.0/10
4. [Apple Announces M5, M5 Pro, and M5 Max Chips with New Fusion Architecture](#item-4) ⭐️ 8.0/10
5. [Simon Willison discusses agentic engineering and AI adoption stages at Pragmatic Summit](#item-5) ⭐️ 7.0/10
6. [NASA watchdog warns Artemis program lacks lunar rescue capability and faces lander technical risks](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Scientists achieve vitrification and functional recovery of adult mouse brain tissue](https://www.pnas.org/doi/10.1073/pnas.2516848123) ⭐️ 9.0/10

Researchers have successfully vitrified and functionally recovered adult mouse brain slices and in-situ whole brains, as published in PNAS. They developed a novel cryoprotectant solution called V3 and optimized the cooling protocol to avoid ice crystal damage, enabling stable preservation below the glass transition temperature. This represents a major breakthrough in cryobiology and neuroscience, demonstrating for the first time that complex adult mammalian brain tissue can be vitrified and retain functional neural activity and synaptic plasticity after rewarming. It opens a new path for preserving brain tissue with its intricate functional architecture, with potential long-term implications for neuroscience research, brain banking, and future medical technologies. The rewarmed brain slices restored cellular metabolism and maintained electrophysiological activity and synaptic plasticity. For whole-brain preservation, the team used vascular perfusion techniques to balance dehydration and cryoprotectant penetration, achieving preliminary functional preservation of the in-situ whole brain.

telegram · zaihuapd · Mar 15, 08:30

**Background**: Vitrification is a cryopreservation technique that rapidly cools a biological sample to form an amorphous, glass-like solid, thereby avoiding the damaging ice crystals that form during conventional slow freezing. Cryoprotectants are chemicals added to biological samples to protect cells from freezing damage. The glass transition temperature (Tg) is a critical point below which the material enters a stable, glassy state, crucial for long-term preservation. Vascular perfusion is a method of delivering cryoprotectants uniformly through an organ's circulatory system, which is particularly challenging for the brain due to the blood-brain barrier.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vitrification">Vitrification - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11753176/">Cryopreservation of brain cell structure: a review - PMC</a></li>

</ul>
</details>

**Tags**: `#cryobiology`, `#neuroscience`, `#vitrification`, `#brain-preservation`, `#PNAS`

---

<a id="item-2"></a>
## [Jazzband Python Project Shuts Down Due to AI-Generated Spam PRs](https://simonwillison.net/2026/Mar/14/jannis-leidel/#atom-everything) ⭐️ 8.0/10

The Jazzband open-source collective announced on March 14, 2026, that it is sunsetting its operations. The decision was driven by GitHub's 'slopocalypse'—a flood of AI-generated spam pull requests and issues—which made its open membership model with shared push access unsustainable. This shutdown highlights a systemic threat to the sustainability of open-source projects that rely on open collaboration. It demonstrates how AI-generated spam is forcing projects to abandon inclusive models, potentially reducing community contributions and increasing maintainer burnout across the ecosystem. Jazzband cited specific data points: only 1 in 10 AI-generated PRs meets project standards, and the curl project had to shut down its bug bounty program because confirmation rates dropped below 5%. GitHub's own response included introducing a 'kill switch' to disable pull requests entirely for affected repositories.

rss · Simon Willison · Mar 14, 18:41

**Background**: Jazzband was an open community that maintained Python-based projects, operating on a model where any member could gain push access to repositories. The term 'slopocalypse' refers to the overwhelming volume of low-quality, AI-generated content (like pull requests and issues) flooding platforms. This phenomenon has become a major pain point for open-source maintainers, forcing them to spend excessive time filtering spam instead of productive work.

<details><summary>References</summary>
<ul>
<li><a href="https://jazzband.co/">Jazzband - We are all part of this</a></li>
<li><a href="https://unprecedented.ghost.io/archive/the-ai-slopocalypse/">The AI Slopocalypse</a></li>
<li><a href="https://prevhq.com/blog/the-open-source-spam-apocalypse">The Open Source Spam Apocalypse (And How to Survive It)</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#ai-spam`, `#github`, `#maintenance`, `#sustainability`

---

<a id="item-3"></a>
## [Glassworm Attack Uses Invisible Unicode Characters to Compromise Over 151 GitHub Repos](https://www.tomshardware.com/tech-industry/cyber-security/malicious-packages-using-invisible-unicode-found-in-151-github-repos-and-vs-code) ⭐️ 8.0/10

Security researchers from Aikido Security have uncovered the Glassworm attack campaign, which uses invisible Unicode characters, specifically zero-width spaces, to hide malicious payloads within code. This technique has compromised at least 151 GitHub repositories, npm packages, and VS Code extensions, including projects like Wasmer and Reworm. This attack is significant because it exploits a fundamental weakness in human code review processes, making malicious code virtually invisible to developers. It represents a sophisticated supply-chain attack that can steal credentials and cryptocurrency tokens, potentially affecting downstream users of compromised open-source projects. The malicious payloads are designed to steal user credentials and crypto tokens, and the attackers use the Solana blockchain as a command-and-control (C2) channel, making it harder to shut down. Researchers also suspect that attackers used large language models (LLMs) to generate code refactoring and version updates that match the style of the targeted projects, increasing the deception.

telegram · zaihuapd · Mar 15, 01:28

**Background**: Zero-width Unicode characters, such as U+200B (Zero Width Space), are non-printing characters that render as invisible spaces in text. They have legitimate uses in text formatting but can be abused in cybersecurity to create homograph attacks or hide malicious code, as they are not easily detectable by human reviewers. Supply-chain attacks target software dependencies (like npm packages) to compromise a wide range of downstream applications. Solana is a high-performance blockchain platform that supports smart contracts and decentralized applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-width_space">Zero-width space - Wikipedia</a></li>
<li><a href="https://www.promptfoo.dev/blog/invisible-unicode-threats/">The Invisible Threat: How Zero-Width Unicode Characters Can Silently Backdoor Your AI-Generated Code | Promptfoo</a></li>
<li><a href="https://www.cisa.gov/news-events/alerts/2025/09/23/widespread-supply-chain-compromise-impacting-npm-ecosystem">Widespread Supply Chain Compromise Impacting npm Ecosystem</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#supply-chain-attack`, `#unicode`, `#github`, `#npm`

---

<a id="item-4"></a>
## [Apple Announces M5, M5 Pro, and M5 Max Chips with New Fusion Architecture](https://t.me/zaihuapd/40272) ⭐️ 8.0/10

Apple has announced its next-generation M5 series of chips, including the M5, M5 Pro, and M5 Max, which feature a new 'Fusion Architecture' design that combines two dies into a single System on a Chip (SoC). The M5 Pro and M5 Max are equipped with an 18-core CPU, consisting of 6 'super cores' and 12 'performance cores,' promising significant performance gains for professional workloads. This marks a major architectural shift for Apple Silicon, moving from a monolithic die to a multi-die 'Fusion' design, which could allow for greater scalability, performance, and efficiency in high-end MacBook Pro models. The introduction of a new core naming scheme and a claimed performance leap reinforces Apple's push to dominate the professional laptop market with its custom silicon. The new 'super cores' appear to be a rebranding of the previous generation's performance cores, while the new 'performance cores' are likely improved efficiency cores, creating a three-tier CPU core hierarchy. The Fusion Architecture represents a departure from Apple's traditional single-die SoC approach, potentially enabling more specialized core configurations and higher core counts.

telegram · zaihuapd · Mar 15, 07:20

**Background**: Apple Silicon refers to the family of custom system-on-a-chip (SoC) processors designed by Apple for its Mac computers, integrating CPU, GPU, memory, and other components onto a single chip for high performance and power efficiency. Prior to the M5, Apple's chips used a unified architecture with two types of CPU cores: high-performance 'P-cores' and energy-efficient 'E-cores,' all fabricated on a single piece of silicon. A System on a Chip (SoC) is an integrated circuit that consolidates all or most components of a computer or electronic system, such as the processor, memory, and input/output ports, into a single chip.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/tyson_cung/apple-m5-fusion-architecture-explained-two-dies-one-chip-infinite-possibilities-o9e">Apple M5 Fusion Architecture Explained - Two... - DEV Community</a></li>
<li><a href="https://www.macworld.com/article/3077260/what-the-hell-is-an-m5-super-core.html">M5 deep dive: What the hell is a super core? | Macworld</a></li>
<li><a href="https://en.wikipedia.org/wiki/System_on_a_chip">System on a chip - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#apple-silicon`, `#hardware`, `#macbook`, `#soc`, `#performance`

---

<a id="item-5"></a>
## [Simon Willison discusses agentic engineering and AI adoption stages at Pragmatic Summit](https://simonwillison.net/2026/Mar/14/pragmatic-summit/#atom-everything) ⭐️ 7.0/10

Simon Willison shared highlights from his fireside chat at the Pragmatic Summit in San Francisco, where he outlined the stages of AI adoption for developers and discussed practical patterns for agentic engineering. He specifically mentioned his transition to AI agents writing more code than him about six months ago and his current use of test-driven development (TDD) with agents. This discussion provides a concrete framework for developers navigating the shift towards AI-assisted coding, highlighting both the potential and the critical trust challenges involved. As companies like StrongDM push towards fully automated 'software factories', understanding these adoption patterns and responsible practices becomes essential for the future of software development. Willison emphasized that using red-green TDD with agents (e.g., by instructing them with 'use red-green TDD') significantly increases the chances of getting working code. He also noted that Opus 4.5 was the first AI model that earned his trust for certain well-understood problem classes, like building a JSON API.

rss · Simon Willison · Mar 14, 18:19

**Background**: Agentic engineering refers to patterns and practices for effectively using AI coding agents, where the agent takes an active role in generating and sometimes executing code. The Pragmatic Summit is a one-day conference hosted by Gergely Orosz and The Pragmatic Engineer, focusing on practical engineering topics. Statsig, whose representative hosted the chat, is a product development platform offering experimentation and feature management tools, recently valued at $1.1 billion.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Feb/23/agentic-engineering-patterns/">Writing about Agentic Engineering Patterns</a></li>
<li><a href="https://www.pragmaticsummit.com/">The Pragmatic Summit</a></li>
<li><a href="https://statsig.com/">Statsig | The modern product development platform</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Agentic Engineering`, `#Developer Tools`, `#AI Adoption`

---

<a id="item-6"></a>
## [NASA watchdog warns Artemis program lacks lunar rescue capability and faces lander technical risks](https://futurism.com/space/nasa-oig-rescue-lunar-astronauts-emergency) ⭐️ 7.0/10

A NASA Office of Inspector General (OIG) report published in March 2026 revealed that the Artemis program has 'ruled out' developing emergency rescue capabilities for astronauts stranded on the Moon during early crewed missions. The report also identified significant technical risks with SpaceX's Starship Human Landing System (HLS), including its requirement for at least 10 propellant transfer missions, limited tilt tolerance on landing, and a single-point-of-failure elevator system for crew egress. This highlights critical, unmitigated safety gaps in NASA's flagship return-to-the-Moon program, directly challenging its 'safety-first' principles for crewed exploration. The identified risks with the commercial landers, particularly SpaceX's complex refueling architecture and lack of redundancy, could lead to further schedule delays, cost overruns, or even mission failure for the pivotal Artemis III landing. The OIG report states NASA has no capability to rescue astronauts from space or the lunar surface if a lander encounters a catastrophic event. For SpaceX's Starship HLS, specific concerns include its 171-foot height making it prone to tipping on the rugged lunar south pole, and the 115-foot elevator being the only way for crew to reach the surface, with no backup ingress/egress method.

telegram · zaihuapd · Mar 15, 02:09

**Background**: NASA's Artemis program aims to return humans to the Moon, with Artemis III targeting a crewed landing near the lunar south pole. The program relies heavily on commercial partners: SpaceX was awarded the contract to develop the Starship HLS, and Blue Origin is developing an alternative lander. Starship HLS is a variant of SpaceX's fully reusable spacecraft, but its massive size requires it to be refueled by multiple 'tanker' Starship flights in low Earth orbit before it can travel to the Moon—a complex operation never before demonstrated at the required scale.

<details><summary>References</summary>
<ul>
<li><a href="https://oig.nasa.gov/news/artemis-lander-program-faces-schedule-delays-and-unmitigated-crew-safety-risks/">Artemis Lander Program Faces Schedule Delays and Unmitigated ...</a></li>
<li><a href="https://news.quantosei.com/2026/03/11/nasa-and-spacex-disagree-about-manual-controls-for-lunar-lander/">NASA & SpaceX Battle Over Crucial Lunar Lander Manual Controls - QuantoSei News</a></li>
<li><a href="https://gist.ly/youtube-summarizer/spacex-orbital-refueling-blue-origins-lunar-landers-explained">SpaceX Orbital Refueling & Blue Origin's Lunar Landers Explained</a></li>

</ul>
</details>

**Tags**: `#space-exploration`, `#systems-engineering`, `#risk-management`, `#nasa`, `#spacex`

---