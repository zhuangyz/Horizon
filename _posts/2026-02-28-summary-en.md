---
layout: default
title: "Horizon Summary: 2026-02-28 (EN)"
date: 2026-02-28
lang: en
---

> From 24 items, 8 important content pieces were selected

---

1. [Anthropic Refuses Pentagon Demands for AI in Surveillance and Autonomous Killing](#item-1) ⭐️ 9.0/10
2. [Security Expert Urges Developers to Stop Using Passkeys for Data Encryption](#item-2) ⭐️ 8.0/10
3. [AI coding skeptic attempts ambitious port of scikit-learn to Rust using AI agents](#item-3) ⭐️ 8.0/10
4. [ChatGPT Nears 1 Billion Weekly Active Users, Surpasses 50 Million Paid Subscribers](#item-4) ⭐️ 8.0/10
5. [QingLong Panel Compromised by .fullgc Mining Malware, Causing 800% CPU Usage](#item-5) ⭐️ 8.0/10
6. [Google Chrome Automatically Downloads 4GB Local AI Model Gemini Nano by Default](#item-6) ⭐️ 7.0/10
7. [South Korean Tax Service Exposes Hardware Wallet Seed Phrase, Leading to $4.8M Crypto Transfer](#item-7) ⭐️ 7.0/10
8. [Leaked Motorola presentation hints at GrapheneOS partnership, first non-Pixel device possible by 2027](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic Refuses Pentagon Demands for AI in Surveillance and Autonomous Killing](https://notdivided.org/) ⭐️ 9.0/10

AI company Anthropic publicly refused to comply with new U.S. Department of War (DoW) contract terms that would allow its AI models to be used for domestic mass surveillance and fully autonomous lethal weapons. This refusal has led to the Trump administration reportedly blacklisting Anthropic and ordering the federal government to stop using its technology. This confrontation sets a major precedent for corporate responsibility in AI ethics, directly challenging government attempts to deploy advanced AI for controversial domestic and military applications. It forces a public debate on the limits of state power, the role of tech companies in national security, and the ethical red lines for autonomous systems that can kill. The specific demands Anthropic refused involved loosening guardrails on its AI models to allow for "any lawful use," which the company interpreted as encompassing domestic surveillance and autonomous killing. In contrast, OpenAI has reportedly reached an agreement with the DoW to deploy its models within the department's classified network, with claims of 'no domestic mass surveillance'.

hackernews · BloondAndDoom · Feb 28, 00:54

**Background**: Large AI models can significantly lower the cost and increase the scale of automated surveillance, making mass monitoring more feasible. Autonomous Weapon Systems (AWS) are machines that can select and engage targets without human intervention, raising profound ethical and legal questions about delegating life-and-death decisions to algorithms. The U.S. Department of War, sometimes referenced in this context, is likely a colloquial or historical reference to the Department of Defense (the Pentagon).

<details><summary>References</summary>
<ul>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/886082/ai-vs-the-pentagon-killer-robots-mass-surveillance-and-red-lines">AI vs. the Pentagon: killer robots, mass surveillance, and red lines | The Verge</a></li>
<li><a href="https://www.cnbc.com/2026/02/27/trump-anthropic-ai-pentagon.html">Trump admin blacklists Anthropic; AI firm refuses Pentagon demands</a></li>
<li><a href="https://www.hindustantimes.com/world-news/us-news/no-domestic-mass-surveillance-whats-inside-openai-deal-dow-trump-admin-anthropic-ai-tussle-101772250629771.html">'No domestic mass surveillance': What's inside OpenAI's deal with Trump admin amid Anthropic tussle | Hindustan Times</a></li>

</ul>
</details>

**Discussion**: Community sentiment is strongly supportive of Anthropic's stance but deeply concerned about broader implications. Key viewpoints include fear of government overreach and the abuse of procurement rules to punish disloyal companies, warnings about the global precedent set by domestic surveillance policies, and concerns that eliminating Anthropic will damage trust in the U.S. tech ecosystem.

**Tags**: `#ai-ethics`, `#government-surveillance`, `#autonomous-weapons`, `#corporate-responsibility`, `#national-security`

---

<a id="item-2"></a>
## [Security Expert Urges Developers to Stop Using Passkeys for Data Encryption](https://simonwillison.net/2026/Feb/27/passkeys/#atom-everything) ⭐️ 8.0/10

Security expert Tim Cappalli has issued a public plea to the identity industry to stop promoting and using passkeys for encrypting user data. This warning highlights the critical risk of permanent, unrecoverable data loss when users inevitably lose their passkeys. This matters because a growing trend of using passkeys for client-side encryption, enabled by features like the WebAuthn PRF extension, creates a systemic risk of data loss at scale. Developers who follow this pattern are building systems where user data becomes permanently inaccessible if a passkey is lost, misplacing the security benefits of passkeys for authentication. The warning specifically targets the misuse of the WebAuthn Pseudo-Random Function (PRF) extension, which allows passkeys to generate deterministic encryption keys. A key caveat is that passkeys, unlike passwords, are device-bound cryptographic key pairs where the private key is not designed to be backed up or recovered in the same way, making key loss catastrophic for encrypted data.

rss · Simon Willison · Feb 27, 22:49

**Background**: Passkeys are a passwordless authentication technology based on the WebAuthn standard, using public-key cryptography. For authentication, a user's private key stays on their device (like a phone or security key), and only a public key is shared with the website. The WebAuthn PRF (Pseudo-Random Function) extension is a newer feature that allows a passkey to also generate a consistent cryptographic key, which some developers are repurposing for client-side data encryption.

<details><summary>References</summary>
<ul>
<li><a href="https://bitwarden.com/blog/prf-webauthn-and-its-role-in-passkeys/">PRF WebAuthn and its role in passkeys | Bitwarden</a></li>
<li><a href="https://www.corbado.com/blog/passkeys-prf-webauthn">Passkeys & WebAuthn PRF for End-to-End Encryption (2026)</a></li>
<li><a href="https://bitwarden.com/resources/passkey-vs-password-whats-the-difference/">Passkey vs password: What's the difference? - Bitwarden</a></li>

</ul>
</details>

**Tags**: `#security`, `#authentication`, `#passkeys`, `#cryptography`, `#usability`

---

<a id="item-3"></a>
## [AI coding skeptic attempts ambitious port of scikit-learn to Rust using AI agents](https://simonwillison.net/2026/Feb/27/ai-agent-coding-in-excessive-detail/#atom-everything) ⭐️ 8.0/10

Developer and AI coding skeptic Max Woolf conducted a detailed experiment using AI coding agents, starting with simple tasks and culminating in an ambitious attempt to port Python's scikit-learn machine learning library to Rust, creating a project tentatively named 'rustlearn'. The experiment tested models like Opus 4.6 and Codex 5.3, which he found to be an order of magnitude better than previous coding LLMs. This experiment demonstrates a significant leap in the practical capabilities of AI coding agents, moving beyond simple code generation to potentially automating complex, large-scale software engineering projects like library porting. It signals a potential paradigm shift in developer workflows, where AI agents could substantially accelerate development cycles and tackle ambitious cross-language or cross-platform projects that were previously considered too time-consuming. The 'rustlearn' project aims not only to implement standard ML algorithms like logistic regression and k-means clustering in Rust but also to match or exceed the performance of scikit-learn's implementations. The author notes the difficulty in communicating the dramatic improvement of recent models without sounding like hype, as they consistently handle complex tasks that would take a human developer months to complete.

rss · Simon Willison · Feb 27, 20:43

**Background**: AI coding agents are autonomous or semi-autonomous software tools that use large language models (LLMs) to understand, generate, and sometimes execute code based on natural language instructions. Scikit-learn is a foundational, open-source Python library for machine learning, widely considered the 'gold standard' for data science; it is built on NumPy and SciPy, with performance-critical parts written in Cython. A 'crate' in Rust is the fundamental unit of compilation and packaging, equivalent to a library or package in other languages, managed by the Cargo tool.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Scikit-learn">scikit-learn - Wikipedia</a></li>
<li><a href="https://doc.rust-lang.org/book/ch07-01-packages-and-crates.html">Packages and Crates - The Rust Programming Language</a></li>

</ul>
</details>

**Tags**: `#AI-agents`, `#software-engineering`, `#Rust`, `#machine-learning`, `#developer-tools`

---

<a id="item-4"></a>
## [ChatGPT Nears 1 Billion Weekly Active Users, Surpasses 50 Million Paid Subscribers](https://9to5mac.com/2026/02/27/chatgpt-approaching-1-billion-weekly-active-users/) ⭐️ 8.0/10

OpenAI has disclosed that ChatGPT now has 900 million weekly active users, a 350% increase from 200 million 18 months ago, and is approaching the 1 billion milestone. The platform has also surpassed 50 million individual paid subscribers, representing over 5% of its user base, with record new subscription growth in January and February 2026. These metrics demonstrate ChatGPT's explosive growth and mainstream adoption, solidifying its position as a dominant AI platform. The high number of paying subscribers indicates strong commercial viability and suggests users increasingly rely on its advanced capabilities, which are becoming deeply integrated into major ecosystems like Apple's iOS and developer tools. The growth is partly driven by strategic integrations, including a deep Siri integration in iOS 18 that allows users to access ChatGPT for more in-depth answers. Furthermore, Apple plans to introduce Google Gemini in a future iOS update and has partnered with Anthropic to provide AI coding support in Xcode 26.3, expanding ChatGPT's reach within the Apple ecosystem.

telegram · zaihuapd · Feb 28, 03:23

**Background**: ChatGPT is a large language model (LLM) developed by OpenAI, capable of generating human-like text, answering questions, and assisting with various tasks. Apple Intelligence is a suite of AI features integrated into Apple's operating systems. Siri is Apple's built-in voice assistant. Xcode is Apple's integrated development environment (IDE) used for creating software for Apple platforms. Agentic coding, as introduced in Xcode 26.3, refers to a development paradigm where AI agents (like those from Anthropic and OpenAI) assist or automate parts of the coding process.

<details><summary>References</summary>
<ul>
<li><a href="https://support.apple.com/guide/iphone/use-chatgpt-with-apple-intelligence-iph00fd3c8c2/ios">Use ChatGPT with Apple Intelligence on iPhone - Apple Support</a></li>
<li><a href="https://www.apple.com/newsroom/2026/02/xcode-26-point-3-unlocks-the-power-of-agentic-coding/">Xcode 26.3 unlocks the power of agentic coding - Apple</a></li>
<li><a href="https://vertu.com/ai-tools/apple-siri-google-gemini-integration-ai-revolution-coming-to-ios-in-2026/">Apple Siri Google Gemini Integration 2026 | Specs & Rollout</a></li>

</ul>
</details>

**Tags**: `#AI`, `#ChatGPT`, `#User Metrics`, `#Platform Integration`, `#Industry Trends`

---

<a id="item-5"></a>
## [QingLong Panel Compromised by .fullgc Mining Malware, Causing 800% CPU Usage](https://t.me/zaihuapd/39934) ⭐️ 8.0/10

On February 7, 2026, multiple users reported that QingLong Panel, a popular task scheduling tool, was compromised by a mining malware named .fullgc, causing abnormal server CPU usage to spike to 800%. The malware achieves persistence by tampering with the config.sh configuration file and can automatically download malicious programs based on the system architecture. This is a significant security incident because QingLong Panel is widely used for server automation, meaning many public-facing servers could be compromised for cryptojacking, leading to severe performance degradation and increased operational costs. The attack highlights the risks associated with exposed management interfaces and the ongoing threat of cryptocurrency mining malware targeting popular open-source tools. Security analysis indicates the malware belongs to the SusMiner family and primarily connects to XMR (Monero) mining pools for illicit cryptocurrency mining. The primary attack targets are servers exposed to public IPv4 environments, and users are advised to check for hidden files in the /ql/data/db/ directory.

telegram · zaihuapd · Feb 28, 13:16

**Background**: QingLong Panel is an open-source timed task management platform that supports Python3, JavaScript, Shell, and TypeScript, often deployed via Docker for automating scripts and jobs. Cryptojacking malware, like this SusMiner variant, secretly hijacks a victim's computing resources to mine cryptocurrencies such as Monero (XMR), which is favored for its privacy features. Persistence mechanisms allow malware to survive reboots, often by modifying system files or configurations.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/whyour/qinglong">GitHub - whyour/qinglong: 支持 Python3、JavaScript、Shell ...</a></li>
<li><a href="https://www.pcrisk.com/removal-guides/12913-xmr-miner-virus">XMR Miner Virus - Easy removal steps (updated)</a></li>

</ul>
</details>

**Tags**: `#security`, `#malware`, `#server-security`, `#cryptojacking`, `#open-source-security`

---

<a id="item-6"></a>
## [Google Chrome Automatically Downloads 4GB Local AI Model Gemini Nano by Default](https://winaero.com/google-chrome-secretly-downloads-huge-local-ai-models/) ⭐️ 7.0/10

Google Chrome has been found to automatically download a roughly 4GB local AI model file named 'weights.bin' by default. This file powers built-in browser AI features like the Prompt API, translation, and summarization. This move signifies a major push by Google to integrate powerful, on-device AI directly into the browser, prioritizing speed and privacy for AI features. However, the automatic download without clear user consent raises significant concerns about transparency, control over disk space usage, and the precedent it sets for software behavior. The model file is associated with Gemini Nano, a compact version of Google's Gemini LLM family designed for on-device use. Users can disable the feature via experimental flags and manually delete the file to free up space, but doing so will cause the related AI features to stop working.

telegram · zaihuapd · Feb 28, 05:02

**Background**: Gemini is a family of multimodal large language models (LLMs) developed by Google DeepMind, succeeding models like LaMDA and PaLM 2. Chrome's Prompt API is a developer interface that allows web applications to send natural language requests to these local AI models, enabling features like chatbots and content summarization that can work offline. The 'weights.bin' file is a common format for storing the learned parameters (weights) of a neural network model.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(language_model)">Gemini (language model ) - Wikipedia</a></li>
<li><a href="https://developer.chrome.com/docs/ai/prompt-api">The Prompt API | AI on Chrome | Chrome for Developers</a></li>
<li><a href="https://medium.com/@ch.mittendorf/navigating-model-weight-file-formats-safetensors-bin-pt-hdf5-and-beyond-97266a621bdf">Navigating Model Weight File Formats: .safetensors, .bin, .pt, HDF5 ...</a></li>

</ul>
</details>

**Tags**: `#Google Chrome`, `#Local AI`, `#Privacy`, `#Browser`, `#Gemini`

---

<a id="item-7"></a>
## [South Korean Tax Service Exposes Hardware Wallet Seed Phrase, Leading to $4.8M Crypto Transfer](https://www.mk.co.kr/cn/stock/11974731) ⭐️ 7.0/10

South Korea's National Tax Service (NTS) accidentally published the full seed phrase of a seized Ledger hardware wallet in a press release, leading to the unauthorized transfer of 4 million PRTG tokens worth approximately $4.8 million. The tokens were returned to the original wallet about 20 hours later. This incident highlights a critical and fundamental security failure by a government agency in handling seized digital assets, undermining public trust in institutional cryptocurrency management. It exposes systemic vulnerabilities in procedures for securing sensitive cryptographic information, with potential implications for legal seizures and asset security worldwide. The exposed wallets, at least three of which had been inactive since January 2023, collectively held 40% of the total PRTG token supply. PRTG has extremely low liquidity, trading only on MEXC with a daily volume around $332, meaning a sale of just $59 could cause a 2% price drop.

telegram · zaihuapd · Feb 28, 11:27

**Background**: A seed phrase (or recovery phrase) is a series of words generated by a cryptocurrency wallet that provides full access to the funds stored within it. Hardware wallets like Ledger are physical devices designed to keep seed phrases offline and secure, making the digital exposure of a seed phrase a catastrophic security breach. The fundamental rule of cryptocurrency self-custody is to never share or digitally store the seed phrase.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ledger.com/academy/hardwarewallet/best-ways-to-protect-your-recovery-phrase">How to Keep Your Seed Phrase Secure - Ledger</a></li>
<li><a href="https://decrypt.co/359404/ethereum-tokens-swiped-returned-south-korean-tax-service">Ethereum Tokens Swiped, Returned After South Korean Tax ... - Decrypt</a></li>

</ul>
</details>

**Tags**: `#cryptocurrency`, `#security`, `#government`, `#blockchain`, `#hardware-wallet`

---

<a id="item-8"></a>
## [Leaked Motorola presentation hints at GrapheneOS partnership, first non-Pixel device possible by 2027](https://grapheneos.social/@GrapheneOS/116115497756691311) ⭐️ 7.0/10

A leaked internal Motorola presentation slide, originally posted on Reddit, explicitly lists GrapheneOS within the company's security features section, strongly suggesting a partnership. The GrapheneOS project later confirmed on Mastodon that an official OEM partner announcement is scheduled for March 2026, with a device planned for release in 2027. This represents a potential major expansion for GrapheneOS beyond its exclusive support for Google Pixel devices, significantly increasing its accessibility and market presence. A partnership with a major OEM like Motorola, which is owned by Lenovo and has a strong focus on enterprise security, could lend substantial legitimacy to the privacy-focused OS and accelerate its adoption in business and security-conscious consumer markets. The leaked slide was quickly deleted by moderators on the r/GrapheneOS subreddit but had already spread widely. Neither GrapheneOS nor Motorola has issued an official statement regarding the leak, and the information remains unconfirmed by the companies involved.

telegram · zaihuapd · Feb 28, 12:38

**Background**: GrapheneOS is a privacy and security-focused mobile operating system based on the Android Open Source Project (AOSP), known for its hardened security features and default privacy protections. It has historically been officially supported only on a select range of Google Pixel devices due to their strong hardware security capabilities. Motorola Solutions, under Lenovo, offers enterprise mobility management and security solutions like 'moto-safe' for business customers, positioning itself in the secure mobile device market.

<details><summary>References</summary>
<ul>
<li><a href="https://www.allthingssecured.com/identity-protection/android-vs-grapheneos-compared/">Android vs GrapheneOS: Privacy, Security & Features Compared</a></li>
<li><a href="https://www.reddit.com/r/GrapheneOS/comments/1r7m2q9/grapheneos_project_member_confirms_oem_partner/">GrapheneOS project member confirms OEM Partner unveil in March 2026</a></li>
<li><a href="https://www.motorola.com/business/moto-safe">moto-safe - Motorola</a></li>

</ul>
</details>

**Tags**: `#mobile-security`, `#privacy`, `#operating-systems`, `#hardware`, `#android`

---