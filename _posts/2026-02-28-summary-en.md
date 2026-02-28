---
layout: default
title: "Horizon Summary: 2026-02-28 (EN)"
date: 2026-02-28
lang: en
---

> From 24 items, 8 important content pieces were selected

---

1. [AI Companies Face Ethical Crossroads Over Government Surveillance and Military Partnerships](#item-1) ⭐️ 8.0/10
2. [Security Expert Urges Developers to Stop Using Passkeys for Data Encryption](#item-2) ⭐️ 8.0/10
3. [Skeptic Tests AI Coding Agents by Attempting to Port scikit-learn to Rust](#item-3) ⭐️ 8.0/10
4. [ChatGPT Nears 1 Billion Weekly Active Users, Surpasses 50 Million Paid Subscribers](#item-4) ⭐️ 8.0/10
5. [Google Chrome downloads 4GB local AI model Gemini Nano by default](#item-5) ⭐️ 7.0/10
6. [South Korea's National Tax Service accidentally leaks hardware wallet seed phrase, leading to $4.8M crypto transfer](#item-6) ⭐️ 7.0/10
7. [Leaked Motorola presentation reveals GrapheneOS partnership, first non-Pixel devices potentially launching in 2027](#item-7) ⭐️ 7.0/10
8. [QingLong Panel Targeted by .fullgc Mining Malware, CPU Usage Spikes to 800%](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [AI Companies Face Ethical Crossroads Over Government Surveillance and Military Partnerships](https://notdivided.org/) ⭐️ 8.0/10

A public discussion has emerged, centered on the website notdivided.org, highlighting growing concerns about AI companies collaborating with government surveillance programs and entering into military technology partnerships. The conversation specifically references OpenAI's reported deal with the Pentagon and questions the ethical frameworks surrounding such collaborations. This matters because the integration of advanced AI into surveillance and military systems raises profound questions about privacy, civil liberties, and the weaponization of technology. The decisions made by leading AI companies now will set precedents for corporate responsibility, government overreach, and the global norms governing dual-use AI technologies. The discussion points to a specific, reported agreement between OpenAI and the U.S. Department of Defense, which allegedly includes ethical safeguards. Critics argue such partnerships could normalize mass surveillance capabilities and expand the use of AI in warfare, despite stated ethical principles from entities like the DOD.

hackernews · BloondAndDoom · Feb 28, 00:54

**Background**: Artificial Intelligence (AI) refers to computer systems that can perform tasks typically requiring human intelligence. Government surveillance programs use technology to monitor populations, often for security purposes. In recent years, AI capabilities like facial recognition and predictive analytics have significantly enhanced the scale and efficiency of such surveillance. Many technology companies face ethical dilemmas when their products are sought for military or intelligence applications, balancing innovation, profit, and social responsibility.

<details><summary>References</summary>
<ul>
<li><a href="https://www.politico.com/news/2026/02/28/openai-announces-new-deal-with-pentagon-including-ethical-safeguards-00805546">OpenAI announces new deal with Pentagon — including ethical safeguards</a></li>
<li><a href="https://www.brookings.edu/articles/how-ai-can-enable-public-surveillance/">How AI can enable public surveillance</a></li>
<li><a href="https://www.war.gov/News/Releases/Release/Article/2091996/dod-adopts-ethical-principles-for-artificial-intelligence/">DOD Adopts Ethical Principles for Artificial Intelligence</a></li>

</ul>
</details>

**Discussion**: Community sentiment is critical and concerned, highlighting hypocrisy and potential dangers. Key viewpoints include: criticism of OpenAI's perceived closeness to the "Department of War" despite public ethical stances; fears that surveillance capabilities developed for the U.S. could be adopted by other countries against American citizens; and concerns that government procurement rules could be weaponized to punish companies for political reasons. Some comments suggest a retaliatory logic, warning that those requesting surveillance AI could themselves become targets.

**Tags**: `#AI Ethics`, `#Government Surveillance`, `#Military Technology`, `#Corporate Responsibility`, `#National Security`

---

<a id="item-2"></a>
## [Security Expert Urges Developers to Stop Using Passkeys for Data Encryption](https://simonwillison.net/2026/Feb/27/passkeys/#atom-everything) ⭐️ 8.0/10

Security expert Tim Cappalli issued a public plea to the identity industry, urging developers to stop using passkeys to encrypt user data. He warns that this practice risks permanent data loss because users frequently lose their passkeys and may not realize their data is irreversibly encrypted. This warning highlights a critical misuse of a core authentication technology that could lead to widespread, irreversible data loss for end-users. It matters because it pushes back against a growing trend of using the WebAuthn PRF extension for client-side encryption, emphasizing that passkeys should remain focused on their primary, secure role as phishing-resistant authentication credentials. The warning specifically targets the use of the WebAuthn Pseudo-Random Function (PRF) extension, which allows passkeys to generate deterministic encryption keys. A key caveat is that the WebAuthn API is designed to prevent direct access to or manipulation of private keys, making key recovery impossible if the passkey (the authenticator holding the private key) is lost.

rss · Simon Willison · Feb 27, 22:49

**Background**: Passkeys are a passwordless authentication technology based on the WebAuthn standard, using public-key cryptography where a public key is stored by the service and a private key is securely stored on a user's device (like a phone or security key). The WebAuthn PRF extension is a feature that allows these passkeys to generate consistent cryptographic keys, which some developers have begun using for client-side data encryption. Unlike traditional password managers which store and manage secrets, passkeys are primarily designed for proving identity during login.

<details><summary>References</summary>
<ul>
<li><a href="https://bitwarden.com/blog/prf-webauthn-and-its-role-in-passkeys/">PRF WebAuthn and its role in passkeys | Bitwarden</a></li>
<li><a href="https://www.corbado.com/blog/passkeys-prf-webauthn">Passkeys & WebAuthn PRF for End-to-End Encryption (2026)</a></li>
<li><a href="https://github.com/w3c/webauthn/issues/1595">Can the private keys be used for other cryptographic operations? · Issue #1595 · w3c/webauthn</a></li>

</ul>
</details>

**Tags**: `#security`, `#authentication`, `#passkeys`, `#cryptography`, `#usability`

---

<a id="item-3"></a>
## [Skeptic Tests AI Coding Agents by Attempting to Port scikit-learn to Rust](https://simonwillison.net/2026/Feb/27/ai-agent-coding-in-excessive-detail/#atom-everything) ⭐️ 8.0/10

In February 2026, AI researcher and skeptic Max Woolf published a detailed account of testing AI coding agents on progressively more ambitious projects, culminating in an attempt to port the core machine learning library scikit-learn from Python to Rust, creating a crate named `rustlearn`. He found that models like Opus 4.6/Codex 5.3 were an order of magnitude better than their predecessors from just months before, successfully handling complex tasks he expected would take months. This real-world, high-stakes test demonstrates a significant leap in the practical capabilities of AI coding agents, moving beyond simple code generation to potentially assisting with large-scale, complex software engineering projects like library porting. It signals a shift where AI agents could become viable tools for accelerating development in performance-critical domains like machine learning, where Rust's speed and safety are advantageous. The project, `rustlearn`, aims not just to replicate scikit-learn's algorithms (like logistic regression and k-means clustering) in Rust, but also to implement faster versions that could outperform the original Python implementations. The author's experience highlights a key frustration: the dramatic improvement in models like Opus 4.6 is so counterintuitively large that it's difficult to communicate without sounding like hype.

rss · Simon Willison · Feb 27, 20:43

**Background**: AI coding agents are AI systems, often built on large language models (LLMs), that can autonomously or semi-autonomously write, refactor, debug, and execute code based on natural language instructions. The landscape in 2026 includes tools like Claude Code, Cursor, and Aider that operate at the repository level. Scikit-learn is a foundational, widely-used Python library for machine learning. Rust is a systems programming language prized for its performance and memory safety, making it an attractive target for porting performance-sensitive Python code.

<details><summary>References</summary>
<ul>
<li><a href="https://www.qodo.ai/blog/best-ai-coding-assistant-tools/">Top 15 AI Coding Assistant Tools to Try in 2026</a></li>
<li><a href="https://github.com/Menonlab-Rich/rsklearn">GitHub - Menonlab-Rich/rsklearn: A collection of sklearn algorithms ...</a></li>
<li><a href="https://lib.rs/crates/rustlearn">rustlearn — system library interface for Rust // Lib.rs</a></li>

</ul>
</details>

**Tags**: `#AI-agents`, `#software-development`, `#Rust`, `#machine-learning`, `#code-generation`

---

<a id="item-4"></a>
## [ChatGPT Nears 1 Billion Weekly Active Users, Surpasses 50 Million Paid Subscribers](https://9to5mac.com/2026/02/27/chatgpt-approaching-1-billion-weekly-active-users/) ⭐️ 8.0/10

OpenAI disclosed that ChatGPT has reached 900 million weekly active users, a 350% increase from 200 million 18 months ago, and is approaching the 1 billion milestone. The platform also surpassed 50 million individual paid subscribers, accounting for over 5% of its user base, with record new subscription growth in January and February 2026. This explosive growth demonstrates ChatGPT's massive mainstream adoption and solidifies its position as a leading consumer AI platform. The significant paid subscriber base, alongside deep integrations with major ecosystems like Apple's iOS and Siri, indicates a successful transition from a free novelty to a sustainable, deeply embedded service with substantial revenue potential. The integration extends beyond ChatGPT, with Apple planning to introduce Google's Gemini in iOS 26.5 and collaborating with Anthropic to provide AI programming support within Xcode. These partnerships highlight a strategic move by Apple to offer a multi-model AI assistant ecosystem rather than relying on a single provider.

telegram · zaihuapd · Feb 28, 03:23

**Background**: ChatGPT is a conversational AI chatbot developed by OpenAI, known for its ability to generate human-like text. Anthropic is an AI safety research company that has developed the Claude family of large language models. Xcode is Apple's integrated development environment (IDE) used for building software for macOS, iOS, and other Apple platforms. The term 'agentic coding' refers to AI tools that can autonomously interact with a development environment to plan, write, and maintain code.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://www.apple.com/newsroom/2026/02/xcode-26-point-3-unlocks-the-power-of-agentic-coding/">Xcode 26.3 unlocks the power of agentic coding - Apple</a></li>
<li><a href="https://en.wikipedia.org/wiki/IOS_26">iOS 26 - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#ChatGPT`, `#User Metrics`, `#Tech Partnerships`, `#Apple Integration`

---

<a id="item-5"></a>
## [Google Chrome downloads 4GB local AI model Gemini Nano by default](https://winaero.com/google-chrome-secretly-downloads-huge-local-ai-models/) ⭐️ 7.0/10

Google Chrome has been discovered automatically downloading a roughly 4GB local AI model file named 'weights.bin' by default. This file is used to power built-in AI features like the Prompt API, translation, and summarization. This represents a significant shift in how major browsers deploy AI, moving towards large-scale, on-device model integration by default. It impacts user storage, privacy expectations, and sets a precedent for silent, automatic downloads of substantial AI assets to enable new browser capabilities. The model is Gemini Nano, Google's on-device foundation model designed for privacy-sensitive and low-latency use cases. Users can disable the feature via experimental flags and delete the file to free up space, but doing so will cause the related AI features to stop working.

telegram · zaihuapd · Feb 28, 05:02

**Background**: Gemini Nano is a lightweight version of Google's Gemini AI model family, optimized to run directly on user devices without requiring a cloud connection. The Prompt API is an experimental web API that allows websites and extensions to access these browser-provided local language models using JavaScript. On-device AI in browsers aims to provide faster responses and enhanced privacy by processing data locally instead of sending it to remote servers.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.android.com/ai/gemini-nano">Gemini Nano | AI | Android Developers</a></li>
<li><a href="https://developer.chrome.com/docs/ai/prompt-api">The Prompt API | AI on Chrome | Chrome for Developers</a></li>
<li><a href="https://www.sitepoint.com/on-device-ai-for-the-web/">Web AI: Everything You Need to Know About On-Device AI for the Web</a></li>

</ul>
</details>

**Tags**: `#Google Chrome`, `#Gemini Nano`, `#On-Device AI`, `#Browser Privacy`, `#AI Deployment`

---

<a id="item-6"></a>
## [South Korea's National Tax Service accidentally leaks hardware wallet seed phrase, leading to $4.8M crypto transfer](https://www.mk.co.kr/cn/stock/11974731) ⭐️ 7.0/10

South Korea's National Tax Service (NTS) accidentally published the complete seed phrase of a seized Ledger hardware wallet in a press release about a tax investigation, which led to the unauthorized transfer of 4 million PRTG tokens worth approximately $4.8 million. Approximately 20 hours later, the tokens were returned to the original wallet address. This incident highlights a critical security failure by a government agency, demonstrating the severe real-world consequences of mishandling cryptocurrency seed phrases. It underscores the importance of proper security protocols for digital assets, even for institutional actors, and raises questions about the competency of authorities dealing with crypto seizures. The leaked seed phrase was from a Ledger hardware wallet, and the image was unredacted. On-chain data shows at least three wallets that had been inactive since January 2023 were affected, collectively holding 40% of the total PRTG supply. PRTG has extremely low liquidity, trading only on MEXC with a daily volume around $332, meaning a sale of just $59 could cause a 2% price drop.

telegram · zaihuapd · Feb 28, 11:27

**Background**: A seed phrase (or recovery phrase) is a series of words that acts as the master key to a cryptocurrency wallet; anyone who possesses it has complete control over the assets. Hardware wallets like Ledger are physical devices designed to store seed phrases offline for enhanced security. The PRTG token (Pre-Retogeum) is a cryptocurrency on the Ethereum ecosystem with a very small market and low trading volume.

<details><summary>References</summary>
<ul>
<li><a href="https://crypto-corner.com/2026/02/23/🛡️-importing-seed-phrase-into-a-hardware-wallet-dos-and-donts/">Importing Seed Phrase Into a Hardware Wallet: Do’s and Don’ts</a></li>
<li><a href="https://www.coingecko.com/en/coins/pre-retogeum">Pre-Retogeum Price: PRTG Live Price Chart, Market Cap & News Today | CoinGecko</a></li>
<li><a href="https://coinmarketcap.com/exchanges/mexc/">MEXC trade volume and market listings | CoinMarketCap</a></li>

</ul>
</details>

**Tags**: `#cryptocurrency`, `#security`, `#government`, `#blockchain`, `#incident`

---

<a id="item-7"></a>
## [Leaked Motorola presentation reveals GrapheneOS partnership, first non-Pixel devices potentially launching in 2027](https://grapheneos.social/@GrapheneOS/116115497756691311) ⭐️ 7.0/10

A leaked internal Motorola presentation slide, originally posted on Reddit's r/GrapheneOS subreddit, explicitly lists GrapheneOS within the company's security features section, strongly suggesting a formal partnership. The GrapheneOS official Mastodon account stated on February 22 that an announcement regarding the OEM partner is scheduled for March 2026, with devices planned for release in 2027. This marks a pivotal expansion for GrapheneOS beyond its long-standing exclusivity to Google Pixel devices, potentially bringing its hardened privacy and security features to a much wider audience through a major smartphone manufacturer. A successful partnership could significantly increase adoption of privacy-focused mobile operating systems, introduce more competition into the secure mobile ecosystem, and challenge the dominance of standard Android in the enterprise and security-conscious consumer markets. The leaked slide was quickly deleted by moderators but had already spread widely, and neither GrapheneOS nor Motorola (owned by Lenovo) has issued an official statement confirming the partnership details. Motorola has been strengthening its enterprise mobile security offerings, holding certifications like Android Enterprise Recommended (AER) and featuring its ThinkShield security platform, which aligns with the potential integration of GrapheneOS.

telegram · zaihuapd · Feb 28, 12:38

**Background**: GrapheneOS is a non-profit, open-source mobile operating system based on Android, renowned for its extreme focus on security and privacy. It has historically been developed and supported almost exclusively for Google Pixel devices due to their robust hardware security features and timely firmware updates. Motorola Solutions (the enterprise-focused arm) and its parent company Lenovo have a significant presence in the business and enterprise mobility market, where device security is a critical selling point.

<details><summary>References</summary>
<ul>
<li><a href="https://www.webpronews.com/grapheneos-expands-to-snapdragon-devices-via-oem-partnership-by-2026/">GrapheneOS Expands to Snapdragon Devices via OEM Partnership by 2026</a></li>
<li><a href="https://reclaimthenet.org/grapheneos-expands-beyond-pixel-phones-with-new-android-partner">GrapheneOS Plans Partnership with Major Android OEM to Expand Beyond ...</a></li>
<li><a href="https://www.motorola.com/us/en/thinkshield">Motorola ThinkShield for Mobile Data Security | Motorola US | motorola</a></li>

</ul>
</details>

**Tags**: `#mobile-security`, `#privacy`, `#open-source`, `#android`, `#mobile-operating-systems`

---

<a id="item-8"></a>
## [QingLong Panel Targeted by .fullgc Mining Malware, CPU Usage Spikes to 800%](https://t.me/zaihuapd/39934) ⭐️ 7.0/10

On February 7, 2026, multiple users reported that QingLong Panel, a popular open-source task scheduling tool, was infected with a mining malware named .fullgc, causing abnormal server CPU usage to spike to 800%. The malware achieves persistence by tampering with the config.sh configuration file and can automatically download malicious programs based on the system architecture. This attack targets a widely-used open-source tool for server automation, posing a significant security risk to system administrators and developers who rely on it. The malware's persistence mechanism and targeting of public-facing servers indicate a sophisticated threat that could lead to substantial resource theft, performance degradation, and increased operational costs for affected organizations. Security agencies have identified the program as belonging to the SusMiner malware family, which primarily connects to XMR (Monero) mining pools for illicit cryptocurrency mining. The main targets are servers exposed to public IPv4 environments, and users are advised to check for hidden files in the /ql/data/db/ directory.

telegram · zaihuapd · Feb 28, 13:16

**Background**: QingLong Panel (GitHub: whyour/qinglong) is an open-source, timed task management platform that supports scripts in Python, JavaScript, and Shell. It is commonly deployed via Docker and used for automating various online tasks, such as checking-in scripts or data fetching. Cryptojacking malware, like this .fullgc variant, secretly hijacks a victim's computing resources to mine cryptocurrency, causing high CPU usage without the owner's consent. The SusMiner family is a known group of malware specifically designed for this purpose.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/whyour/qinglong">GitHub - whyour/ qinglong : 支持 Python3、JavaScript、Shell...</a></li>
<li><a href="https://malpedia.caad.fkie.fraunhofer.de/families">Malware Families</a></li>

</ul>
</details>

**Tags**: `#security`, `#malware`, `#server-security`, `#cryptojacking`, `#open-source`

---