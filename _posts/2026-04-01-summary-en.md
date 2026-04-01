---
layout: default
title: "Horizon Summary: 2026-04-01 (EN)"
date: 2026-04-01
lang: en
---

> From 28 items, 7 important content pieces were selected

---

1. [Axios npm Package Compromised in Supply Chain Attack via Malicious Dependency](#item-1) ⭐️ 9.0/10
2. [Axios npm package compromised via maintainer account hijack, delivering cross-platform RAT](#item-2) ⭐️ 9.0/10
3. [Trump says he's strongly considering US withdrawal from NATO, calls alliance a 'paper tiger'](#item-3) ⭐️ 9.0/10
4. [Visual Guide Analyzes Leaked Claude Code, Revealing AI Agent Architecture](#item-4) ⭐️ 8.0/10
5. [GitHub repository reconstructs Claude Code's TypeScript source from npm package source maps](#item-5) ⭐️ 8.0/10
6. [Paralyzed Man Creates Music Using Brain Implant and Neural Signals](#item-6) ⭐️ 8.0/10
7. [Baidu's Apollo Go Robotaxis Stall on Wuhan Elevated Roads, Trapping Passengers for Hours](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Axios npm Package Compromised in Supply Chain Attack via Malicious Dependency](https://simonwillison.net/2026/Mar/31/supply-chain-attack-on-axios/#atom-everything) ⭐️ 9.0/10

On March 31, 2026, a supply chain attack compromised the widely-used Axios HTTP client npm package, which has over 101 million weekly downloads. The malicious versions 1.14.1 and 0.30.4 included a newly published dependency called `plain-crypto-js` that was designed to steal credentials and install a remote access trojan (RAT). This attack demonstrates the severe risk posed by supply chain attacks on foundational open-source packages, potentially impacting millions of applications and developers downstream. It highlights the critical need for improved publishing security measures, such as trusted publishing, to prevent unauthorized releases from compromised credentials. The attack vector was a leaked, long-lived npm token, not a direct modification of Axios source code. The malicious `plain-crypto-js` package was published as version 4.2.1, following a seemingly clean version 4.2.0 published 18 hours earlier to establish a brief history on the registry.

rss · Simon Willison · Mar 31, 23:28

**Background**: A software supply chain attack occurs when an attacker compromises a third-party component (like a library or dependency) that is used by other software, thereby injecting malicious code into the larger ecosystem that depends on it. npm is the default package manager for the JavaScript runtime Node.js and hosts millions of reusable code packages. Trusted publishing is a security feature that allows package publishers to configure npm to only accept publishes from specific, authorized workflows (like GitHub Actions), reducing the risk from leaked traditional authentication tokens.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack - Wikipedia</a></li>
<li><a href="https://docs.npmjs.com/trusted-publishers/">Trusted publishing for npm packages | npm Docs</a></li>
<li><a href="https://snyk.io/blog/axios-npm-package-compromised-supply-chain-attack-delivers-cross-platform/">Axios npm Package Compromised: Supply Chain Attack Delivers Cross-Platform RAT | Snyk</a></li>

</ul>
</details>

**Tags**: `#security`, `#supply-chain`, `#npm`, `#axios`, `#malware`

---

<a id="item-2"></a>
## [Axios npm package compromised via maintainer account hijack, delivering cross-platform RAT](https://t.me/zaihuapd/40637) ⭐️ 9.0/10

On March 31, 2026, security firm StepSecurity discovered that the npm maintainer account for the popular JavaScript library Axios was hijacked. Attackers manually published two malicious versions (axios@1.14.1 and axios@0.30.4), bypassing the project's GitHub Actions CI/CD pipeline, which injected a dependency that deployed a remote access trojan (RAT) targeting Windows, macOS, and Linux systems. This is a critical supply chain attack affecting Axios, a library with approximately 60 million weekly downloads, giving it a massive potential impact radius across countless web applications and development pipelines. The incident demonstrates how sophisticated attackers can bypass automated security checks by compromising long-lived credentials and manually publishing malicious packages, eroding trust in the npm ecosystem. The attack added a single, never-imported dependency called `plain-crypto-js@^4.2.1`, which was pre-staged by a separate attacker account about 18 hours earlier. This dependency contained a `postinstall` hook script that executed platform-specific payloads, and all traces were designed to self-destruct after execution.

telegram · zaihuapd · Apr 1, 05:25

**Background**: Axios is a widely-used promise-based HTTP client for JavaScript, commonly employed in both browser and Node.js environments. npm (Node Package Manager) is the primary registry for JavaScript packages, where supply chain attacks involve compromising legitimate packages to distribute malware. CI/CD (Continuous Integration/Continuous Deployment) pipelines like GitHub Actions are automated workflows meant to build, test, and deploy code, but they can be bypassed if an attacker gains direct publishing access.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/axios-npm-compromised-maintainer-hijacked-rat">axios compromised on npm: maintainer account hijacked, RAT deployed</a></li>
<li><a href="https://anonhaven.com/en/news/axios-npm-supply-chain-attack-rat/">Axios npm package compromised after maintainer account hijack delivers cross-platform RAT</a></li>
<li><a href="https://snyk.io/blog/axios-npm-package-compromised-supply-chain-attack-delivers-cross-platform/">Axios npm Package Compromised: Supply Chain Attack Delivers Cross-Platform RAT | Snyk</a></li>

</ul>
</details>

**Tags**: `#security`, `#supply-chain`, `#npm`, `#javascript`, `#malware`

---

<a id="item-3"></a>
## [Trump says he's strongly considering US withdrawal from NATO, calls alliance a 'paper tiger'](https://www.telegraph.co.uk/world-news/2026/04/01/donald-trump-strongly-considering-pulling-us-out-of-nato/) ⭐️ 9.0/10

In an interview with The Telegraph, former US President Donald Trump stated he is 'strongly considering' withdrawing the United States from NATO, describing the alliance as a 'paper tiger'. This consideration follows NATO allies' refusal to participate in military action against Iran and to send warships to reopen the Strait of Hormuz. A potential US withdrawal from NATO would represent the most significant shake-up of the transatlantic security architecture since the alliance's founding in 1949, fundamentally undermining collective defense in Europe and global power dynamics. It would signal a dramatic shift from decades of US foreign policy and could embolden adversaries while creating a major crisis of confidence among remaining member states. The immediate trigger was NATO's refusal to support US-led military action in the Strait of Hormuz, which Iran has effectively closed for weeks, disrupting about 20% of global oil shipments. Trump claimed that Russian President Vladimir Putin also understands the organization's weakness, framing the decision as a response to European allies being 'no longer reliable defense partners.'

telegram · zaihuapd · Apr 1, 14:15

**Background**: The North Atlantic Treaty Organization (NATO) is a military alliance established in 1949, with its core principle being collective defense as outlined in Article 5, which states that an attack on one member is an attack on all. The United States has been the alliance's most powerful member and primary security guarantor since its inception. The Strait of Hormuz is a critical maritime chokepoint between the Persian Gulf and the Gulf of Oman, through which a significant portion of the world's seaborne oil exports passes.

**Tags**: `#geopolitics`, `#international-relations`, `#defense-policy`, `#nato`, `#us-foreign-policy`

---

<a id="item-4"></a>
## [Visual Guide Analyzes Leaked Claude Code, Revealing AI Agent Architecture](https://ccunpacked.dev/) ⭐️ 8.0/10

A developer created a visual guide (ccunpacked.dev) to analyze the leaked 500,000-line source code for Anthropic's Claude Code, an AI coding agent. The guide maps the complex architecture and reveals specific defensive programming patterns like "frustration regexes" used to manage LLM behavior. This analysis provides a rare, detailed look into the engineering challenges of making a probabilistic LLM behave reliably in an agent system. It highlights the significant code overhead required for state management, error handling, and security in production AI agents, offering valuable lessons for the broader AI agent development community. The codebase includes patterns like "frustration regexes"—regular expressions designed to detect user frustration from prompts—and extensive sanitization and retry logic for tool calls. The visual guide was created quickly by an independent developer to aid in understanding the large, complex codebase for personal learning and project adaptation.

hackernews · autocracy101 · Apr 1, 05:15

**Background**: Claude Code is an AI-powered coding assistant developed by Anthropic that can autonomously execute tasks by calling tools (like shell commands or code editors) based on natural language instructions. LLM agents are systems where a large language model acts as a "brain," deciding when and how to use external tools to complete multi-step tasks. A key challenge is ensuring deterministic and reliable behavior from inherently probabilistic LLMs, often requiring extensive "defensive programming" to handle edge cases and errors.

<details><summary>References</summary>
<ul>
<li><a href="https://alex000kim.com/posts/2026-03-31-claude-code-source-leak/">The Claude Code Source Leak: fake tools, frustration regexes, undercover mode, and more | Alex Kim's blog</a></li>
<li><a href="https://www.datacamp.com/blog/llm-agents">LLM Agents Explained: Architecture, Frameworks, and Use Cases | DataCamp</a></li>

</ul>
</details>

**Discussion**: The discussion reveals mixed reactions. Some commenters are surprised by the 500k-line codebase's size for a CLI agent, seeing it as evidence of the "state-management nightmare" involved in making LLMs deterministic. Others argue the real value lies in Anthropic's proprietary models, not the agent framework, which they see as a solvable engineering problem. The guide's author stated they built it to adapt ideas into their own projects.

**Tags**: `#ai-agents`, `#reverse-engineering`, `#llm-engineering`, `#software-architecture`, `#anthropic`

---

<a id="item-5"></a>
## [GitHub repository reconstructs Claude Code's TypeScript source from npm package source maps](https://t.me/zaihuapd/40632) ⭐️ 8.0/10

An unofficial GitHub repository named 'claude-code-sourcemap' has reconstructed the TypeScript source code of Claude Code version 2.1.88 by extracting data from the `sourcesContent` field within the `cli.js.map` source map file included in the public npm package @anthropic-ai/claude-code. The reconstruction yielded 4,756 files, including 1,884 .ts and .tsx files. This incident highlights a significant security and intellectual property risk for software publishers, demonstrating how source maps in publicly distributed packages can inadvertently expose proprietary source code. It provides a rare, detailed look into the internal structure of a proprietary AI coding assistant and underscores the importance of secure build and deployment practices for all software, especially in the competitive AI sector. The reconstruction specifically leveraged the optional `sourcesContent` field within the source map, which can embed the original source code directly, eliminating the need for separate source files. The exposed code pertains to version 2.1.88 of Claude Code, and the repository's existence demonstrates the practical application of reverse-engineering tools designed to work with source maps.

telegram · zaihuapd · Apr 1, 02:36

**Background**: Source maps are files that create a mapping between minified/transpiled code (like JavaScript) and the original source code (like TypeScript), aiding in debugging. The optional `sourcesContent` field within a source map can contain the full text of the original sources, embedding them directly into the map file. When such source maps are included in publicly distributed npm packages, they can potentially expose the complete original source code if not properly stripped, a known issue discussed in developer security circles.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/alanwest/your-npm-package-is-leaking-source-code-and-you-probably-dont-know-it-4kf5">Your npm Package Is Leaking Source Code (And You Probably Don't Know It) - DEV Community</a></li>
<li><a href="https://blog.openreplay.com/source-maps-work/">What Are Source Maps and How Do They Work - blog.openreplay.com</a></li>
<li><a href="https://stackoverflow.com/questions/19802462/do-source-maps-include-the-source-text">Do source maps include the source text? - Stack Overflow</a></li>

</ul>
</details>

**Tags**: `#reverse-engineering`, `#ai-systems`, `#source-code-analysis`, `#npm-security`, `#anthropic`

---

<a id="item-6"></a>
## [Paralyzed Man Creates Music Using Brain Implant and Neural Signals](https://www.wired.com/story/meet-the-man-making-music-with-his-brain-implant/) ⭐️ 8.0/10

A 69-year-old tetraplegic man, Galen Buckwalter, who received six Blackrock Neurotech brain implant chips in 2024 as part of a Caltech study, can now generate musical tones directly from his neural signals using a custom algorithm. He used the brain-generated track in a song for his band Siggy's album, released on March 15. This represents a significant expansion of brain-computer interface (BCI) applications beyond basic medical restoration, demonstrating its potential to enhance quality of life and enable creative expression for people with severe disabilities. It highlights a human-centered direction for neurotechnology, focusing on personal agency and long-term user engagement, which is crucial for broader adoption. The system allows Buckwalter to simultaneously control two audio streams with his thoughts. Beyond music creation, the implant also enables him to operate a computer and has restored some sensation in his fingers, showcasing the multi-functional potential of the technology.

telegram · zaihuapd · Apr 1, 07:34

**Background**: Brain-Computer Interfaces (BCIs) are systems that decode neural signals to allow direct communication between the brain and external devices, often used to restore function for individuals with paralysis. Blackrock Neurotech is a leading company in implantable BCI technology, with devices used in over 1000 research labs. Converting neural signals to music involves complex algorithms that interpret brain activity patterns to generate or control musical parameters, a field sometimes referred to as Brain-Computer Music Interfaces (BCMI).

<details><summary>References</summary>
<ul>
<li><a href="https://blackrockneurotech.com/">Blackrock Neurotech | Empowered by Thought</a></li>
<li><a href="https://link.springer.com/article/10.1007/s12559-024-10280-6">NeuralPMG: A Neural Polyphonic Music Generation System Based on Machine Learning Algorithms | Cognitive Computation | Springer Nature Link</a></li>

</ul>
</details>

**Tags**: `#Brain-Computer Interface`, `#Neurotechnology`, `#Human-Computer Interaction`, `#Assistive Technology`, `#Creative AI`

---

<a id="item-7"></a>
## [Baidu's Apollo Go Robotaxis Stall on Wuhan Elevated Roads, Trapping Passengers for Hours](https://www.sznews.com/news/content/2026-03/31/content_32000110.htm) ⭐️ 7.0/10

On the evening of March 31, Baidu's Apollo Go (Luobo Kuaipao) robotaxi service in Wuhan experienced a widespread system failure, causing multiple vehicles to stop suddenly on elevated highways and major roads, trapping passengers inside. The in-car system displayed a "driving system abnormal" alert, and passengers reported extreme difficulty reaching emergency contacts or customer service via the app, with some waiting nearly two hours before being assisted off the highway by traffic police and staff. This incident represents a significant real-world failure of a commercial robotaxi service, highlighting critical vulnerabilities in safety protocols, emergency response, and system resilience. It directly impacts public trust in autonomous vehicle technology and raises urgent questions about the operational readiness and fail-safe mechanisms required for large-scale deployment, especially in complex urban environments like elevated roads. The service provider's customer service initially attributed the failure to "network reasons," but later official客服 representatives claimed to have no knowledge of the Wuhan incident when contacted by press, requesting a vehicle number for inquiry. Notably, the official Apollo Go platform had not released any information about the failure or response measures by the time of reporting.

telegram · zaihuapd · Apr 1, 01:06

**Background**: Baidu's Apollo Go is a commercial robotaxi (autonomous ride-hailing) service operating in several Chinese cities, utilizing the company's Apollo autonomous driving platform. These vehicles rely on a combination of AI, sensors (LiDAR, radar, cameras), and GPS for navigation, and typically require robust network connectivity for certain cloud-based functions and remote monitoring. The term "robotaxi" specifically refers to self-driving cars operated for a ridesharing service, which are designed to function without a human driver in the vehicle.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apollo_Go">Apollo Go - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Self-driving_car">Self-driving car - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#autonomous-vehicles`, `#safety`, `#reliability`, `#robotaxi`, `#incident-report`

---