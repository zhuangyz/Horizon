---
layout: default
title: "Horizon Summary: 2026-04-01 (EN)"
date: 2026-04-01
lang: en
---

> From 26 items, 6 important content pieces were selected

---

1. [OpenAI closes $122B funding round at $852B valuation](#item-1) ⭐️ 9.0/10
2. [Supply Chain Attack Compromises Axios npm Package with Malicious Dependency](#item-2) ⭐️ 9.0/10
3. [Axios npm maintainer account hijacked, malicious versions deliver remote access trojan](#item-3) ⭐️ 9.0/10
4. [Google Quantum AI Reduces Bitcoin Attack Requirements 20x, Enabling Potential 9-Minute Key Extraction](#item-4) ⭐️ 9.0/10
5. [Claude Code source leak reveals 'undercover mode' for hiding AI attribution](#item-5) ⭐️ 8.0/10
6. [Unofficial GitHub repository reconstructs Claude Code's TypeScript source from public npm package source maps](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI closes $122B funding round at $852B valuation](https://www.cnbc.com/2026/03/31/openai-funding-round-ipo.html) ⭐️ 9.0/10

OpenAI announced the closing of its latest funding round, securing $122 billion in committed capital at a post-money valuation of $852 billion. This marks a historic milestone for AI company valuations. This valuation demonstrates massive market confidence in OpenAI's potential and signals a paradigm shift in how the AI industry is valued. It provides the company with unprecedented capital to accelerate development and compete in the rapidly evolving AI landscape. The funding is described as 'committed capital,' which implies it may be contingent on future milestones rather than immediately available cash. OpenAI's reported revenue is approximately $2 billion per month, but this figure is calculated differently than competitors like Anthropic, as OpenAI takes a 20% share of revenue from Azure sales.

hackernews · surprisetalk · Mar 31, 20:07

**Background**: OpenAI is a leading artificial intelligence research and deployment company, known for creating models like GPT-4 and the widely used ChatGPT. A funding round is a process where a company raises capital from investors in exchange for equity, and the 'post-money valuation' is the company's estimated worth after the new investment has been added. In recent years, AI companies have seen valuations soar as the technology's commercial potential becomes clearer.

**Discussion**: Community discussion reveals skepticism about the funding structure, with users noting the term 'committed capital' suggests conditional promises rather than immediate cash. There is also debate about revenue growth, with comparisons to Anthropic highlighting different revenue reporting methodologies. Some express concern about the sheer scale of the valuation and limited public investment access, while others interpret the emphasis on ChatGPT's consumer reach as a response to competitive pressure in the enterprise market.

**Tags**: `#AI`, `#Venture Capital`, `#OpenAI`, `#Business`, `#Valuation`

---

<a id="item-2"></a>
## [Supply Chain Attack Compromises Axios npm Package with Malicious Dependency](https://simonwillison.net/2026/Mar/31/supply-chain-attack-on-axios/#atom-everything) ⭐️ 9.0/10

A supply chain attack compromised versions 1.14.1 and 0.30.4 of the popular Axios HTTP client npm package by adding a malicious dependency called plain-crypto-js. This newly published malware was designed to steal credentials and install a remote access trojan (RAT). This attack is highly significant because Axios is a foundational JavaScript library with over 101 million weekly downloads, meaning the potential impact is massive across the software ecosystem. It highlights the critical vulnerability of widely-used open-source packages to supply chain attacks and underscores the urgent need for more secure publishing practices. The attack appears to have originated from a leaked, long-lived npm authentication token. A notable detection heuristic is that the malicious packages were published without an accompanying GitHub release, a pattern also seen in a recent attack on the LiteLLM package.

rss · Simon Willison · Mar 31, 23:28

**Background**: A software supply chain attack involves injecting malicious code into a legitimate software component, which then infects all applications that depend on it. npm is the default package manager for the Node.js JavaScript runtime and hosts millions of open-source packages. Trusted publishing is a modern security feature that replaces traditional token-based authentication, often using mechanisms like OpenID Connect (OIDC) to ensure packages are only published from authorized, automated workflows (like GitHub Actions).

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack - Wikipedia</a></li>
<li><a href="https://docs.npmjs.com/about-access-tokens">About access tokens - npm Docs</a></li>
<li><a href="https://docs.npmjs.com/packages-and-modules/contributing-packages-to-the-registry/">Contributing packages to the registry | npm Docs</a></li>

</ul>
</details>

**Tags**: `#security`, `#supply-chain`, `#npm`, `#axios`, `#malware`

---

<a id="item-3"></a>
## [Axios npm maintainer account hijacked, malicious versions deliver remote access trojan](https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan) ⭐️ 9.0/10

On March 31, 2026, the npm account of the lead axios maintainer was compromised, leading to the manual publication of two malicious package versions: axios@1.14.1 and axios@0.30.4. These versions introduced a malicious dependency, plain-crypto-js, which executed a script to deploy a cross-platform remote access trojan (RAT) that connected to a command-and-control (C2) server. This is a significant supply chain attack targeting a foundational JavaScript library with over 300 million weekly downloads, posing a massive risk to countless applications and developers. The sophistication of the attack, which bypassed automated security checks and targeted multiple operating systems, highlights the growing threat of credential compromise in open-source ecosystems. The malware was designed for stealth, automatically deleting its malicious scripts post-execution and forging clean configuration files to evade security audits. The malicious dependency `plain-crypto-js@4.2.1` was pinned to a version that was not yet uploaded at the time of the axios release, a tactic to bypass scanners that would find nothing suspicious until the malicious package was later published.

telegram · zaihuapd · Mar 31, 04:10

**Background**: Axios is a widely used, promise-based HTTP client for JavaScript, commonly employed in both Node.js and browser environments to make network requests. A supply chain attack in software occurs when an attacker compromises a component, tool, or service that is trusted and used by many downstream projects, allowing malware to be distributed indirectly. The npm (Node Package Manager) registry is the primary repository for JavaScript packages, and account hijackings there can have cascading security impacts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/axios-npm-compromised-maintainer-hijacked-rat">axios compromised on npm: maintainer account hijacked, RAT deployed</a></li>
<li><a href="https://www.wiz.io/blog/axios-npm-compromised-in-supply-chain-attack">Axios NPM Distribution Compromised in Supply Chain Attack | Wiz Blog</a></li>
<li><a href="https://www.stepsecurity.io/blog/axios-compromised-on-npm-malicious-versions-drop-remote-access-trojan">axios Compromised on npm - Malicious Versions Drop Remote Access Trojan - StepSecurity</a></li>

</ul>
</details>

**Tags**: `#security`, `#supply-chain-attack`, `#npm`, `#javascript`, `#malware`

---

<a id="item-4"></a>
## [Google Quantum AI Reduces Bitcoin Attack Requirements 20x, Enabling Potential 9-Minute Key Extraction](https://research.google/blog/safeguarding-cryptocurrency-by-disclosing-quantum-vulnerabilities-responsibly/) ⭐️ 9.0/10

Google's Quantum AI team published a paper demonstrating a 20x reduction in the quantum computing resources needed to break Bitcoin's elliptic curve cryptography. They compiled two attack circuits requiring fewer than 1200 and 1450 logical qubits, which could enable private key extraction in under 9 minutes after a transaction is broadcast. This represents a paradigm shift in quantum vulnerability assessment, significantly shortening the estimated timeline for practical attacks on cryptocurrencies. It highlights an urgent need for the crypto ecosystem to transition to quantum-resistant algorithms, as approximately 6.9 million BTC (one-third of supply) are potentially at risk due to exposed public keys. The optimized Shor's algorithm circuits could run on superconducting quantum computers with fewer than 500,000 physical qubits, compared to prior estimates of ~10 million. An attacker has about a 41% chance of stealing funds before transaction confirmation (within Bitcoin's ~10-minute block time), with early network wallets (~1.7 million BTC) being particularly vulnerable.

telegram · zaihuapd · Mar 31, 08:03

**Background**: Bitcoin's security relies on Elliptic Curve Cryptography (ECC), where private keys generate public keys and addresses. Shor's algorithm is a quantum algorithm that can solve the mathematical problems (like the discrete logarithm problem for ECC) underlying this cryptography exponentially faster than classical computers. Logical qubits are error-corrected computational units built from many noisy physical qubits, which are the basic hardware components susceptible to decoherence and errors.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Shor's_algorithm">Shor's algorithm - Wikipedia</a></li>
<li><a href="https://quantumai.google/static/site-assets/downloads/cryptocurrency-whitepaper.pdf">Securing Elliptic Curve Cryptocurrencies against Quantum ...</a></li>
<li><a href="https://www.forbes.com/sites/digital-assets/2026/03/31/google-finds-quantum-computers-could-break-bitcoin-sooner-than-expected/">Google Finds Quantum Computers Could Break Bitcoin Sooner ...</a></li>

</ul>
</details>

**Tags**: `#quantum-computing`, `#cryptocurrency-security`, `#cryptography`, `#blockchain`, `#quantum-cryptanalysis`

---

<a id="item-5"></a>
## [Claude Code source leak reveals 'undercover mode' for hiding AI attribution](https://alex000kim.com/posts/2026-03-31-claude-code-source-leak/) ⭐️ 8.0/10

The entire 512,000-line TypeScript source code for Anthropic's Claude Code tool was accidentally leaked via a source map file included in its public npm package. The leaked code reveals internal practices including an 'undercover mode' designed to prevent the AI from revealing its identity in commit messages and PR descriptions. This leak exposes the internal mechanics and strategic practices of a major AI company's development tool, raising significant questions about AI transparency, attribution ethics in software development, and corporate security practices. It also highlights the tension between using AI to assist in open-source contributions and the desire to conceal that assistance. The leak occurred because a 59.8 MB `.map` source map file for debugging was included in version 2.1.88 of the `@anthropic-ai/claude-code` npm package. The 'undercover mode' explicitly instructs the AI to never include phrases like 'Claude Code' or 'Co-Authored-By: Claude' in commits, effectively hiding AI-generated code attribution.

hackernews · alex000kim · Mar 31, 13:04

**Background**: Claude Code is an AI-powered coding assistant tool developed by Anthropic. A source map file is a debugging aid that maps minified/transpiled code back to its original source code; if included in a public release, it can expose the original source. The leak follows another recent incident where Anthropic's 'Mythos' model details were accidentally exposed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibtimes.co.uk/claude-code-leak-advanced-ai-secrets-1789623">Anthropic Claude Code Leak Reveals Secrets—Self-Healing ...</a></li>
<li><a href="https://dev.to/gabrielanhaia/claude-codes-entire-source-code-was-just-leaked-via-npm-source-maps-heres-whats-inside-cjo">Claude Code's Entire Source Code Was Just Leaked via npm ...</a></li>
<li><a href="https://venturebeat.com/technology/claude-codes-source-code-appears-to-have-leaked-heres-what-we-know">Claude Code's source code appears to have leaked: here's what ...</a></li>

</ul>
</details>

**Discussion**: Community discussion reveals high engagement, with debates centering on the ethics of the 'undercover mode,' Anthropic's aggressive DMCA takedown of related GitHub forks, and concerns about a pattern of security lapses. Some commenters are amazed at the level of internal 'trade secrets' and business context openly commented in the code, while others question the impact on user trust.

**Tags**: `#ai-ethics`, `#source-code-leak`, `#software-development`, `#anthropic`, `#security`

---

<a id="item-6"></a>
## [Unofficial GitHub repository reconstructs Claude Code's TypeScript source from public npm package source maps](https://github.com/ChinaSiro/claude-code-sourcemap) ⭐️ 8.0/10

An unofficial GitHub repository named 'claude-code-sourcemap' has reconstructed 4,756 TypeScript source files from Anthropic's Claude Code version 2.1.88 by extracting the original source code from the `sourcesContent` field within a publicly accessible source map file (`cli.js.map`) included in the npm package `@anthropic-ai/claude-code`. The repository includes 1,884 `.ts` and `.tsx` files covering modules like CLI entry points, tools, commands, services, plugins, voice interaction, and Vim mode. This incident highlights a significant security oversight where sensitive proprietary source code can be inadvertently exposed through debugging artifacts like source maps included in production npm packages. It serves as a critical reminder for engineering teams to audit their build and deployment pipelines to prevent unintentional source code disclosure, which could aid competitors or malicious actors in understanding and potentially exploiting the software's architecture. The repository maintainer explicitly states that the reconstructed code is derived from publicly released packages and source map analysis, does not represent the official internal development repository structure, and is for research purposes only. A prominent warning in the repository advises users not to link Claude Code to this repo, as the remote URL hash included in reported information could lead to account risks.

telegram · zaihuapd · Mar 31, 09:33

**Background**: Source maps are files that map minified or transpiled code (like JavaScript) back to its original source code (like TypeScript), primarily to aid debugging in browser developer tools. They often contain a `sourcesContent` field which can embed the full original source code. When such source map files are included in publicly distributed npm packages, they can be used to reverse-engineer and reconstruct the original, readable source code, effectively leaking the codebase if not properly stripped during the production build process.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/gabrielanhaia/claude-codes-entire-source-code-was-just-leaked-via-npm-source-maps-heres-whats-inside-cjo">Claude Code's Entire Source Code Was Just Leaked via npm ...</a></li>
<li><a href="https://stackoverflow.com/questions/32383865/how-to-use-sourcemaps-to-restore-the-original-file">javascript - How to use sourcemaps to restore the... - Stack Overflow</a></li>
<li><a href="https://wellstsai.com/en/post/restoring-source-code-from-sourcemaps/">Restoring Frontend Source Code Using Sourcemaps: Practical ...</a></li>

</ul>
</details>

**Tags**: `#reverse-engineering`, `#source-maps`, `#anthropic`, `#claude`, `#security`

---