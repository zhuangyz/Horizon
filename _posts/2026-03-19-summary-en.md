---
layout: default
title: "Horizon Summary: 2026-03-19 (EN)"
date: 2026-03-19
lang: en
---

> From 15 items, 6 important content pieces were selected

---

1. [SEC Approves Nasdaq to Trade Tokenized Securities](#item-1) ⭐️ 9.0/10
2. [OpenAI acquires Astral, the company behind popular Python tools uv and Ruff.](#item-2) ⭐️ 8.0/10
3. [Apple's 'LLM in a Flash' technique runs 397B Qwen model locally on a MacBook Pro.](#item-3) ⭐️ 8.0/10
4. [Snowflake Cortex AI Agent Vulnerable to Sandbox Escape via Prompt Injection](#item-4) ⭐️ 8.0/10
5. [OpenAI announces acquisition of Astral, developer of Python tools uv and Ruff, to integrate into Codex ecosystem.](#item-5) ⭐️ 8.0/10
6. [Mozilla to launch free built-in VPN in Firefox 149 with 50GB monthly data cap](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [SEC Approves Nasdaq to Trade Tokenized Securities](https://www.reuters.com/legal/government/nasdaq-receives-sec-nod-trading-tokenized-securities-2026-03-18/) ⭐️ 9.0/10

The U.S. Securities and Exchange Commission (SEC) has formally approved Nasdaq's proposal to allow the trading of tokenized securities for specific stocks on its exchange. This approval, granted on March 18, 2026, permits Nasdaq to utilize blockchain technology to offer these tokenized assets for trading on the same platform as traditional shares. This is a historic regulatory milestone that bridges traditional finance with blockchain technology, potentially transforming stock trading and settlement. It represents institutional adoption at the highest level and could significantly enhance the efficiency, transparency, and global interoperability of capital markets. The tokenized assets will share the same ticker symbol as their corresponding traditional stock and confer identical shareholder rights. The Depository Trust & Clearing Corporation (DTCC) will be responsible for the clearing and settlement of these tokenized securities, integrating them into the existing trusted financial infrastructure.

telegram · zaihuapd · Mar 19, 11:45

**Background**: Tokenized securities are traditional financial assets, such as stocks or bonds, that are digitally represented on a blockchain or distributed ledger. The Depository Trust & Clearing Corporation (DTCC) is the world's largest securities settlement system and has been actively exploring blockchain integration, including plans for digital cash settlement by 2027. Nasdaq's proposal, initially filed in September 2025, aimed to fuse traditional stock trading with blockchain-based settlement on its core platform.

<details><summary>References</summary>
<ul>
<li><a href="https://coinmarketcap.com/academy/glossary/tokenized-securities">Tokenized Securities Definition - CoinMarketCap</a></li>
<li><a href="https://cryptotreasuryinsights.substack.com/p/dtcc-eyes-2027-digital-cash-settlement">DTCC Eyes 2027 Digital Cash Settlement, Ethereum Remains in Play</a></li>
<li><a href="https://crypto.news/nasdaq-wins-sec-approval-to-trial-tokenized-stock-trading/">Nasdaq wins SEC approval to trial tokenized stock trading</a></li>

</ul>
</details>

**Tags**: `#blockchain`, `#financial-regulation`, `#tokenization`, `#traditional-finance`, `#securities-trading`

---

<a id="item-2"></a>
## [OpenAI acquires Astral, the company behind popular Python tools uv and Ruff.](https://astral.sh/blog/openai) ⭐️ 8.0/10

OpenAI has announced its acquisition of Astral, the company responsible for developing the high-performance Python tools uv (a package manager) and Ruff (a linter/formatter). This move brings key open-source developer infrastructure under the control of a major AI corporation. This acquisition is significant because it represents a trend of large AI companies consolidating control over foundational developer tools, raising concerns about the future openness, sustainability, and direction of critical open-source projects within the Python ecosystem. Astral's tools, uv and Ruff, are written in Rust and are known for being extremely fast drop-in replacements for traditional Python tools like pip, Flake8, and Black. The acquisition announcement has not specified detailed plans for the future governance or licensing of these projects.

hackernews · ibraheemdev · Mar 19, 13:05

**Background**: Astral is a company focused on building high-performance developer tools for Python. Its flagship products are uv, an extremely fast Python package and project manager written in Rust, and Ruff, an equally fast linter and code formatter also written in Rust. Both tools have gained rapid adoption in the Python community for their speed and ability to replace multiple existing tools. OpenAI is a leading artificial intelligence research and deployment company.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/astral-sh/uv">GitHub - astral-sh/uv: An extremely fast Python package and project manager, written in Rust. · GitHub</a></li>
<li><a href="https://docs.astral.sh/ruff/linter/">The Ruff Linter - Astral</a></li>

</ul>
</details>

**Discussion**: The community reaction is predominantly one of concern and sadness. Commenters express anxiety about the future openness of the tools, the risk of vendor lock-in, and the broader trend of corporate consolidation of the "means of production" in software development. While some congratulate the Astral team, there is widespread worry about the tools' dependence on a capital-intensive company like OpenAI.

**Tags**: `#acquisition`, `#open-source`, `#python`, `#developer-tools`, `#ecosystem`

---

<a id="item-3"></a>
## [Apple's 'LLM in a Flash' technique runs 397B Qwen model locally on a MacBook Pro.](https://simonwillison.net/2026/Mar/18/llm-in-a-flash/#atom-everything) ⭐️ 8.0/10

Researcher Dan Woods successfully implemented techniques from Apple's 'LLM in a Flash' paper to run the massive 397-billion-parameter Qwen3.5-397B-A17B model on a 48GB MacBook Pro M3 Max, achieving a speed of over 5.5 tokens per second by streaming expert weights from the SSD. He used an 'autoresearch' pattern with Claude Code to generate MLX Objective-C and Metal code after running 90 experiments. This demonstrates a practical path to running state-of-the-art, massive language models on consumer-grade hardware with limited memory, significantly lowering the barrier to high-performance local AI. It validates Apple's memory optimization research and shows how Mixture-of-Experts architectures can be leveraged for efficient edge deployment. The model's expert weights were quantized to 2-bit, while non-expert components like embeddings stayed at full precision, keeping 5.5GB resident in RAM. The number of active experts per token was reduced from the model's usual 10 to 4, with the researcher noting the biggest quality drop occurred at 3 experts.

rss · Simon Willison · Mar 18, 23:56

**Background**: Apple's 'LLM in a Flash' is a 2023 research paper that addresses running LLMs larger than available DRAM by storing parameters in flash memory (SSD) and loading them on-demand. Key techniques include 'windowing' to reuse activated neurons and 'row-column bundling' to read larger, contiguous chunks from flash. A Mixture-of-Experts (MoE) model like Qwen3.5-397B-A17B consists of many 'expert' sub-networks; for each input token, only a small subset of these experts is activated, which makes streaming weights from slower storage feasible.

<details><summary>References</summary>
<ul>
<li><a href="https://machinelearning.apple.com/research/efficient-large-language">LLM in a Flash: Efficient Large Language Model Inference with Limited Memory - Apple Machine Learning Research</a></li>
<li><a href="https://arxiv.org/abs/2312.11514">[2312.11514] LLM in a flash: Efficient Large Language Model Inference with Limited Memory</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>

</ul>
</details>

**Tags**: `#LLM Optimization`, `#Edge AI`, `#Mixture-of-Experts`, `#Memory Efficiency`, `#Apple Research`

---

<a id="item-4"></a>
## [Snowflake Cortex AI Agent Vulnerable to Sandbox Escape via Prompt Injection](https://simonwillison.net/2026/Mar/18/snowflake-cortex-ai/#atom-everything) ⭐️ 8.0/10

Security researchers from PromptArmor discovered a critical vulnerability in Snowflake's Cortex AI agent, where a prompt injection attack hidden in a GitHub repository README tricked the agent into executing malicious shell code. The attack exploited process substitution in a `cat` command, bypassing the agent's allow-list security controls and escaping its sandbox to download and execute malware. This incident demonstrates a concrete and severe attack chain where prompt injection directly leads to a full sandbox escape and remote code execution in a major cloud platform's AI service. It highlights the inherent risks of relying on allow-list-based command filtering for AI agents and underscores the urgent need for more robust, deterministic sandboxing solutions across the rapidly expanding field of AI-powered automation. The specific exploit used Bash process substitution (`<(...)`) to nest commands, allowing a seemingly safe `cat` command to execute a `wget` that downloaded and ran a remote script. The vulnerability has since been fixed by Snowflake. The researcher's commentary suggests that allow-lists for command patterns are inherently unreliable and advocates for sandboxes that operate outside the agent's control layer.

rss · Simon Willison · Mar 18, 17:43

**Background**: Snowflake Cortex is a suite of AI services within the Snowflake Data Cloud, and Cortex Agents are AI assistants that can perform tasks like analyzing code or data. Prompt injection is a technique where malicious instructions are hidden within seemingly normal user input to manipulate an AI model's behavior. A sandbox is a security mechanism that restricts a program's access to system resources, and a sandbox escape occurs when code breaks out of these restrictions. Process substitution is a Bash shell feature that allows the output of a command to be treated like a file, enabling complex command chaining.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Process_substitution">Process substitution - Wikipedia</a></li>
<li><a href="https://simonwillison.net/2026/Mar/18/snowflake-cortex-ai/">Snowflake Cortex AI Escapes Sandbox and Executes Malware</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#ai-security`, `#prompt-injection`, `#sandbox-escape`, `#cloud-security`, `#vulnerability`

---

<a id="item-5"></a>
## [OpenAI announces acquisition of Astral, developer of Python tools uv and Ruff, to integrate into Codex ecosystem.](https://openai.com/index/openai-to-acquire-astral) ⭐️ 8.0/10

OpenAI announced it will acquire Astral, the open-source Python tooling company behind the widely-used uv package manager and Ruff linter/formatter. Following the acquisition, Astral's team will join OpenAI's Codex team, and its toolchain will be integrated into the Codex ecosystem to enable AI agents to directly utilize these developer tools. This acquisition represents a strategic move by OpenAI to deeply integrate high-performance, modern developer tools directly into its AI-assisted coding platform, Codex. It could significantly enhance the capabilities of AI coding assistants by giving them direct access to the same fast, reliable toolchain that millions of Python developers already use for tasks like dependency management, linting, and formatting. The acquisition is pending regulatory approval, and until it closes, OpenAI and Astral will operate independently. OpenAI also reported that its Codex platform has seen a 3x growth in users and a 5x growth in usage since the beginning of the year, now boasting over 2 million weekly active users.

telegram · zaihuapd · Mar 19, 13:46

**Background**: Astral is a company focused on building high-performance developer tools for the Python ecosystem. Its flagship products are uv, an extremely fast Python package and project manager written in Rust that serves as a modern replacement for pip, and Ruff, an extremely fast Python linter and code formatter, also written in Rust, which aims to be a drop-in replacement for tools like Flake8, isort, and Black. OpenAI's Codex is a platform for AI-assisted software development, powering tools that help with coding tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/astral-sh/uv">GitHub - astral-sh/uv: An extremely fast Python package and project manager, written in Rust. · GitHub</a></li>
<li><a href="https://docs.astral.sh/ruff/">Ruff - Astral Docs</a></li>
<li><a href="https://astral.sh/">Astral: High-performance Python tooling</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Python`, `#Developer Tools`, `#AI-Assisted Coding`, `#Acquisition`

---

<a id="item-6"></a>
## [Mozilla to launch free built-in VPN in Firefox 149 with 50GB monthly data cap](https://cybernews.com/privacy/mozilla-launch-free-vpn-firefox-march/?utm_source=flipboard&amp;utm_content=CyberNews_com%2Fmagazine%2FLatest+cybersecurity+news) ⭐️ 7.0/10

Mozilla announced it will introduce a free, built-in VPN feature in Firefox 149, starting March 24, 2026. The feature will initially roll out to users in France, Germany, the UK, and the US, offering 50GB of monthly data for browser traffic. This move significantly lowers the barrier to entry for basic online privacy by integrating a VPN directly into a major web browser at no cost. It represents a strategic shift for Mozilla in the competitive browser privacy space and could pressure other browser vendors to offer similar built-in protections. The built-in VPN works by routing browser traffic through a proxy server to mask the user's IP address and location. Importantly, it only protects traffic within the Firefox browser itself and does not secure traffic from other applications on the user's device.

telegram · zaihuapd · Mar 19, 11:00

**Background**: A VPN, or Virtual Private Network, encrypts a user's internet connection and routes it through a remote server, hiding their real IP address and location from websites and potential eavesdroppers. Browser-based VPNs, like the one Mozilla is introducing, are a specific type that only secures traffic within the web browser, unlike traditional VPN applications that protect all traffic from a device. Mozilla already offers a separate, full-device subscription VPN service called Mozilla VPN, which uses the WireGuard protocol.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomsguide.com/computing/vpns/a-free-built-in-vpn-is-coming-to-firefox-and-you-wont-even-need-an-extension">A free, built-in VPN is coming to Firefox – and you won't ...</a></li>
<li><a href="https://cybernews.com/privacy/mozilla-launch-free-vpn-firefox-march/">Mozilla launches free Firefox VPN with 50GB limit| Cybernews</a></li>
<li><a href="https://www.ipvanish.com/blog/browser-vpn/">Browser VPN vs Real VPN : What You’re Actually Getting | IPVanish</a></li>

</ul>
</details>

**Tags**: `#browser-privacy`, `#firefox`, `#vpn`, `#web-security`

---