---
layout: default
title: "Horizon Summary: 2026-04-02 (EN)"
date: 2026-04-02
lang: en
---

> From 25 items, 7 important content pieces were selected

---

1. [NASA's Artemis II crew mission successfully launches to the Moon.](#item-1) ⭐️ 9.0/10
2. [Axios npm maintainer account hijacked, malicious versions inject cross-platform RAT](#item-2) ⭐️ 9.0/10
3. [Paralyzed Man Composes Music Using Brain Implant, Releases Album Track](#item-3) ⭐️ 8.0/10
4. [GitHub repository reverse-engineers Anthropic's Claude Code from source maps in public npm package](#item-4) ⭐️ 8.0/10
5. [NASA's Artemis 2 Crewed Lunar Mission Enters Final Countdown for Historic Launch](#item-5) ⭐️ 8.0/10
6. [Rising DRAM Prices Threaten Hobbyist Single-Board Computer Market](#item-6) ⭐️ 7.0/10
7. [Cloudflare announces EmDash, a TypeScript-based CMS with sandboxed plugin security](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [NASA's Artemis II crew mission successfully launches to the Moon.](https://www.nasa.gov/blogs/missions/2026/04/01/live-artemis-ii-launch-day-updates/) ⭐️ 9.0/10

NASA's Artemis II mission, carrying a crew of astronauts, successfully launched on April 1, 2026, marking humanity's first crewed lunar mission in over 50 years. The mission will perform a lunar flyby before returning to Earth for a splashdown on April 10. This launch is a critical milestone for NASA's Artemis program, paving the way for a sustained human presence on the Moon and serving as a stepping stone for future Mars exploration. It demonstrates the operational readiness of key systems like the Space Launch System (SLS) rocket and Orion spacecraft for deep space crewed missions. The mission will test Orion's life support, navigation, and crew systems in deep space, including critical functions like oxygen regulation and carbon dioxide removal. Following this mission, the focus shifts to developing capabilities like propellant transfer (via SpaceX's Starship) and lunar landers (like Blue Origin's Blue Moon) to enable the subsequent Artemis III lunar landing mission.

hackernews · apitman · Apr 1, 17:11

**Background**: The Artemis program is NASA's initiative to return humans to the Moon and establish a sustainable presence there. Its core architecture relies on the Space Launch System (SLS), a super heavy-lift rocket, to launch the crewed Orion spacecraft. Orion is designed for deep space missions, featuring advanced life support systems to keep astronauts safe during long-duration flights beyond Earth orbit.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Artemis_program">Artemis program - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Space_Launch_System">Space Launch System - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Orion_(spacecraft)">Orion (spacecraft) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community expressed awe at the mission's technological achievements, such as the incredible launch speed mentioned by one user. A key discussion point centered on the mission's broader value, with some defending space exploration as a noble endeavor that drives progress and inspires humanity, while others referenced concerns about technical risks like the heat shield. There was also forward-looking discussion about the next steps in the Artemis program, including the development of Starship and lunar landers.

**Tags**: `#space-exploration`, `#nasa`, `#artemis-program`, `#space-technology`, `#human-spaceflight`

---

<a id="item-2"></a>
## [Axios npm maintainer account hijacked, malicious versions inject cross-platform RAT](https://t.me/zaihuapd/40637) ⭐️ 9.0/10

On March 30-31, 2026, security firm StepSecurity discovered that the npm account of a lead maintainer of the axios JavaScript library was hijacked. The attacker manually published two malicious versions, axios@1.14.1 and axios@0.30.4, which injected a dependency on a malicious package called plain-crypto-js to deploy a cross-platform remote access trojan (RAT). This is a significant software supply chain attack targeting axios, a foundational HTTP client library with approximately 100 million weekly downloads. The attack's sophistication—bypassing CI/CD, targeting multiple OSes, and using a pre-staged dependency—highlights a critical threat to the entire JavaScript/Node.js ecosystem and the security of countless applications that depend on it. The attacker bypassed the project's GitHub Actions CI/CD pipeline by using a stolen, long-lived npm access token to publish directly via the npm CLI. The malicious dependency `plain-crypto-js` was staged 18 hours prior to the attack and its sole purpose was to execute a `postinstall` script that delivered OS-specific RAT payloads, with all traces designed to self-destruct.

telegram · zaihuapd · Apr 1, 05:25

**Background**: Axios is a popular promise-based HTTP client for JavaScript, widely used in both Node.js and browser environments. npm (Node Package Manager) is the default package registry for the JavaScript ecosystem, where libraries like axios are published and installed by developers. A supply chain attack occurs when an attacker compromises a trusted component (like a library) to distribute malware to its users. A Remote Access Trojan (RAT) is malware that provides an attacker with remote control over an infected system.

<details><summary>References</summary>
<ul>
<li><a href="https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan">axios Compromised on npm - Malicious Versions Drop Remote Access Trojan - StepSecurity</a></li>
<li><a href="https://snyk.io/blog/axios-npm-package-compromised-supply-chain-attack-delivers-cross-platform/">Axios npm Package Compromised: Supply Chain Attack Delivers Cross-Platform RAT | Snyk</a></li>
<li><a href="https://www.elastic.co/security-labs/axios-one-rat-to-rule-them-all">Inside the Axios supply chain compromise - one RAT to rule them all — Elastic Security Labs</a></li>

</ul>
</details>

**Tags**: `#security`, `#supply-chain`, `#npm`, `#javascript`, `#malware`

---

<a id="item-3"></a>
## [Paralyzed Man Composes Music Using Brain Implant, Releases Album Track](https://www.wired.com/story/meet-the-man-making-music-with-his-brain-implant/) ⭐️ 8.0/10

Galen Buckwalter, a 69-year-old quadriplegic, can now compose music using neural signals after receiving six Blackrock Neurotech brain implant chips in 2024. The algorithm-assisted tones he generated were used in a song for his band Siggy's album, released on March 15. This represents a significant expansion of brain-computer interface (BCI) applications beyond restoring basic motor or communication functions, demonstrating their potential for creative expression and personal fulfillment. It highlights a shift towards designing neurotechnology that aligns with users' personal interests and quality of life, which is crucial for long-term adoption. The system uses algorithms developed by the research team to translate neural signals into musical tones, allowing Buckwalter to control two audio streams simultaneously. Beyond music, the implant also enables him to operate a computer and has restored some sensation in his fingers.

telegram · zaihuapd · Apr 1, 07:34

**Background**: Brain-computer interfaces (BCIs) are systems that create a direct communication pathway between the brain and an external device, often to restore function for people with paralysis or neurological disorders. Companies like Blackrock Neurotech develop implantable microelectrode arrays that record neural activity; this data is then decoded by algorithms to control computers or prosthetics. Research into Brain-Computer Music Interfacing (BCMI) explores how to extract control information from brain signals and design generative music techniques that respond to it.

<details><summary>References</summary>
<ul>
<li><a href="https://blackrockneurotech.com/">Blackrock Neurotech | Empowered by Thought</a></li>
<li><a href="https://www.researchgate.net/publication/321619139_Guide_to_Brain-Computer_Music_Interfacing">Guide to Brain - Computer Music Interfacing | Request PDF</a></li>

</ul>
</details>

**Tags**: `#brain-computer-interface`, `#neurotechnology`, `#human-computer-interaction`, `#assistive-technology`, `#neuroscience`

---

<a id="item-4"></a>
## [GitHub repository reverse-engineers Anthropic's Claude Code from source maps in public npm package](https://t.me/zaihuapd/40641) ⭐️ 8.0/10

A GitHub repository named 'claude-code-sourcemap' has reverse-engineered the TypeScript source code for Anthropic's Claude Code version 2.1.88 by extracting content from the `sourcesContent` field within a source map file (`cli.js.map`) bundled in the public npm package `@anthropic-ai/claude-code`. The process successfully reconstructed 4,756 files, including 1,884 TypeScript (.ts/.tsx) files. This incident highlights a critical software supply chain vulnerability where proprietary code from a major AI company was inadvertently exposed through a common development artifact. It underscores significant risks for intellectual property protection and raises questions about the security practices of AI tooling, potentially impacting trust in commercial AI products and their deployment pipelines. The exposure occurred because the production npm package included a source map file containing the `sourcesContent` field, which embeds the original source code. The repository was created on March 31, 2026, following a discovery by security researcher Chaofan Shou, and the leaked code was rapidly forked by tens of thousands of users on GitHub.

telegram · zaihuapd · Apr 1, 08:07

**Background**: Source maps are files generated during the build process of web applications (like those using TypeScript or minified JavaScript) to map the transformed, minified code back to the original source code for debugging purposes. The `sourcesContent` field is an optional part of a source map that can contain the full text of the original source files, making them self-contained but also a security risk if included in production bundles. NPM (Node Package Manager) is the primary registry for JavaScript packages, and publishing packages with source maps is a common but often overlooked practice that can lead to source code leakage.

<details><summary>References</summary>
<ul>
<li><a href="https://insiderllm.com/guides/claude-code-source-leak-what-we-learned/">Claude Code's Source Just Leaked: What 500K Lines of... | InsiderLLM</a></li>
<li><a href="https://web.dev/articles/source-maps">What are source maps? | Articles | web.dev</a></li>
<li><a href="https://dev.to/alanwest/your-npm-package-is-leaking-source-code-and-you-probably-dont-know-it-4kf5">Your npm Package Is Leaking Source Code... - DEV Community</a></li>

</ul>
</details>

**Tags**: `#reverse-engineering`, `#source-maps`, `#anthropic`, `#intellectual-property`, `#npm-security`

---

<a id="item-5"></a>
## [NASA's Artemis 2 Crewed Lunar Mission Enters Final Countdown for Historic Launch](https://www.nasa.gov/) ⭐️ 8.0/10

NASA's Artemis 2 mission, the first crewed lunar flight since 1972, is on the launch pad at Kennedy Space Center and preparing for liftoff as early as April 1, 6:24 PM ET. The mission will send four astronauts on a 10-day journey around the Moon aboard the Orion spacecraft, launched by the Space Launch System (SLS) rocket. This mission marks humanity's return to lunar space after more than half a century, representing a critical step in NASA's Artemis program to establish a sustainable human presence on the Moon and serve as a proving ground for future Mars missions. Its success is pivotal for restoring U.S. leadership in deep space exploration and advancing international collaboration in lunar science and exploration. The launch follows multiple technical delays, including a liquid hydrogen leak during fueling tests and an interruption in helium flow to the rocket's upper stage, which forced the vehicle back to the assembly building for repairs in February and March. The mission is a crewed lunar flyby and will not involve a lunar landing; it is designed to test the Orion spacecraft's systems in deep space with astronauts on board.

telegram · zaihuapd · Apr 1, 22:01

**Background**: NASA's Artemis program is a series of missions aimed at returning humans to the Moon and eventually sending astronauts to Mars. The Space Launch System (SLS) is NASA's new super-heavy-lift rocket designed for these deep space missions, while the Orion spacecraft is the crew vehicle. The last human mission to lunar orbit was Apollo 17 in December 1972. The uncrewed Artemis 1 test flight successfully orbited the Moon in late 2022.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/太空發射系統">太空发射系统 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.voachinese.com/a/artemis-ii-march-launch-window-out-of-consideration-after-helium-pressure-system-fault-20260225/8117595.html">由于 氦 气 压力系统 故 障 ，“阿尔忒弥斯二号”3月发射计划推迟 | 美国之音</a></li>

</ul>
</details>

**Tags**: `#space-exploration`, `#nasa`, `#artemis-program`, `#aerospace-engineering`, `#science-news`

---

<a id="item-6"></a>
## [Rising DRAM Prices Threaten Hobbyist Single-Board Computer Market](https://www.jeffgeerling.com/blog/2026/dram-pricing-is-killing-the-hobbyist-sbc-market/) ⭐️ 7.0/10

A blog post by Jeff Geerling highlights that significant increases in DRAM (Dynamic Random-Access Memory) prices are making hobbyist single-board computers (SBCs) like Raspberry Pi less affordable and available. Market analysis from TrendForce forecasts DRAM contract prices could rise 58% to 63% quarter-over-quarter in Q2 2026. This matters because SBCs are crucial for education, prototyping, and DIY projects, and their rising cost could stifle innovation and learning in these areas. Furthermore, the DRAM price surge is a broader supply chain issue that is also forecast to significantly impact the smartphone market and other consumer electronics sectors. The price pressure is not limited to SBCs; comments note vendor quotes for other machines increasing by 50% due to memory and supply chain issues. Some community members also point out that high DRAM costs may push simpler computing tasks back to more cost-effective microcontrollers, representing a potential shift in design philosophy.

hackernews · ingve · Apr 1, 21:36

**Background**: DRAM is a type of volatile memory used as the main working memory in most computers and electronic devices, including SBCs. Single-board computers, like the Raspberry Pi, are complete computers built on a single circuit board, popular for hobbyist projects, education, and embedded applications. The DRAM market is highly concentrated among a few major manufacturers and is sensitive to supply-demand dynamics, manufacturing advancements, and demand from sectors like AI and data centers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/dram/dram-and-nand-contract-prices-to-climb-again-in-q2">DRAM prices predicted to jump 63% in Q2, NAND up to 75% ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Raspberry_Pi">Raspberry Pi - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dynamic_random-access_memory">Dynamic random - access memory - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed, with some users noting that current prices are still far from historical highs, while others emphasize the widespread impact beyond SBCs. Key viewpoints include forecasts of a shrinking smartphone market due to RAM costs, concerns about helium supply issues exacerbating the problem, and observations that cost pressures are forcing a re-evaluation of which tasks truly need SBC-level computing power versus microcontrollers.

**Tags**: `#hardware`, `#supply-chain`, `#single-board-computers`, `#dram`, `#market-trends`

---

<a id="item-7"></a>
## [Cloudflare announces EmDash, a TypeScript-based CMS with sandboxed plugin security](https://blog.cloudflare.com/emdash-wordpress/) ⭐️ 7.0/10

Cloudflare has announced EmDash, a new content management system (CMS) written entirely in TypeScript and built on a serverless architecture. Its key innovation is a sandboxed plugin system using Cloudflare's Dynamic Workers, which isolates plugins to address the fundamental security vulnerabilities inherent in WordPress's plugin architecture. This matters because WordPress powers over 40% of the web, and its plugin ecosystem is a major source of security breaches due to plugins having unrestricted system access. EmDash's architectural approach could set a new standard for CMS security, potentially reducing widespread website compromises and appealing to developers seeking modern, secure, and scalable alternatives. EmDash is built on top of Astro, a fast web framework for content-driven sites, and its plugins are standard TypeScript modules. While it addresses security and modern development workflows, its success will depend on overcoming WordPress's massive network effect and established ecosystem.

hackernews · elithrar · Apr 1, 16:14

**Background**: WordPress is a dominant, PHP-based CMS known for its extensive plugin ecosystem, but this architecture grants plugins full access to the server, creating significant security risks. A sandboxed plugin architecture isolates plugin code, limiting its access to the host system's resources and data to prevent malicious or buggy code from causing harm. TypeScript is a superset of JavaScript that adds static typing, helping catch errors during development and making large codebases more maintainable.

<details><summary>References</summary>
<ul>
<li><a href="https://www.codecentric.de/en/knowledge-hub/blog/plug-in-architectures-webassembly">Plug - in architectures with server-side WebAssembly</a></li>
<li><a href="https://en.wikipedia.org/wiki/TypeScript">TypeScript - Wikipedia</a></li>
<li><a href="https://www.unicon.net/insights/articles/contrasting-system-architectures-an-overview-of-serverless-and-traditional-approaches">System Architecture : Traditional and Serverless CMS Approaches</a></li>

</ul>
</details>

**Discussion**: Community discussion highlights both technical approval and skepticism about adoption. Developers praise the focus on TypeScript and sandboxed Workers as a correct solution to WordPress's security and plugin management woes. However, others argue that WordPress's dominance stems from its ease of use and vast network effect, suggesting that technical superiority alone may not be enough to drive a large-scale migration from the established platform.

**Tags**: `#cms`, `#security`, `#cloudflare`, `#typescript`, `#serverless`

---