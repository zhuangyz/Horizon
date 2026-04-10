---
layout: default
title: "Horizon Summary: 2026-04-10 (EN)"
date: 2026-04-10
lang: en
---

> From 20 items, 4 important content pieces were selected

---

1. [ByteDance launches native full-duplex voice model Seeduplex, now fully deployed in Doubao app](#item-1) ⭐️ 8.0/10
2. [FBI extracts deleted Signal messages from iPhone notification database](#item-2) ⭐️ 8.0/10
3. [macOS kernel bug causes network failure after 49.7 days of uptime, requiring reboot](#item-3) ⭐️ 7.0/10
4. [OpenAI launches $100/month ChatGPT Pro tier with 5x Plus usage limits](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [ByteDance launches native full-duplex voice model Seeduplex, now fully deployed in Doubao app](https://seed.bytedance.com/seeduplex) ⭐️ 8.0/10

ByteDance has officially launched Seeduplex, a native full-duplex large voice model, which is now fully deployed in its Doubao app. This marks the technology's transition from the lab to large-scale production, enabling real-time, high-quality voice interaction for hundreds of millions of users. This represents a significant industry advancement by moving full-duplex voice AI from research to a massive production environment, potentially setting a new standard for natural, human-like conversational AI. It directly impacts hundreds of millions of Doubao users and could accelerate the adoption of real-time voice interfaces across applications. The model achieves true 'listen and speak simultaneously' capability through voice pre-training and reinforcement learning (RL) techniques. It specifically focuses on precise interference suppression and dynamic endpoint detection while maintaining extremely fast response times.

telegram · zaihuapd · Apr 9, 05:35

**Background**: Traditional voice assistant systems typically operate in a 'half-duplex' mode, where the system and user take turns speaking and listening. Full-duplex models, in contrast, are engineered for real-time bidirectional exchange, allowing for overlapping speech, interruptions, and rapid back-and-forth conversation, much like human dialogue. Dynamic endpoint detection is a key technical challenge in such systems, as it involves accurately determining when a user has finished speaking to enable natural turn-taking.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2405.19487">[2405.19487] A Full-duplex Speech Dialogue Scheme Based On Large Language Models</a></li>
<li><a href="https://www.emergentmind.com/topics/full-duplex-spoken-dialogue-model">Full-Duplex Spoken Dialogue Model</a></li>
<li><a href="https://arxiv.org/abs/2210.14252">Dynamic Speech Endpoint Detection with Regression Targets</a></li>

</ul>
</details>

**Tags**: `#speech-recognition`, `#generative-ai`, `#real-time-systems`, `#bytedance`, `#voice-interface`

---

<a id="item-2"></a>
## [FBI extracts deleted Signal messages from iPhone notification database](https://www.404media.co/fbi-extracts-suspects-deleted-signal-messages-saved-in-iphone-notification-database-2/) ⭐️ 8.0/10

During the Prairieland Detention Center trial in Texas, FBI forensic examiners extracted incoming Signal messages that had been deleted from the app by accessing the iPhone's internal notification database. The technique recovered only incoming message previews, not outgoing messages, from the iOS system storage. This reveals a significant forensic vulnerability where encrypted messaging app content can persist on devices via iOS notification previews, potentially undermining user privacy expectations even after message deletion. It highlights a conflict between user convenience features like lock screen previews and the security guarantees of end-to-end encrypted apps. The vulnerability specifically affects Signal when 'Show Previews' is enabled on the lock screen, causing iOS to store message content in its internal notification database. Signal acknowledged a request for comment on March 12 but did not follow up, and Apple did not respond to inquiries.

telegram · zaihuapd · Apr 9, 14:05

**Background**: Signal is a popular end-to-end encrypted messaging app that promises high privacy by ensuring only the sender and recipient can read messages. iOS notifications can display message previews on the lock screen, and to enable this feature, the operating system temporarily stores the preview content in a system-managed database. Digital forensics tools can sometimes extract data from this database, even if the source app has deleted its own copies of the messages.

<details><summary>References</summary>
<ul>
<li><a href="https://discuss.privacyguides.net/t/signal-messages-retrieved-from-ios-notification/36475">Signal messages retrieved from iOS notification - General - Privacy Guides Community</a></li>
<li><a href="https://support.signal.org/hc/en-us/articles/360049673331-Storage-Management">Storage Management - Signal Support</a></li>

</ul>
</details>

**Tags**: `#digital-forensics`, `#privacy`, `#encrypted-messaging`, `#iOS-security`, `#Signal`

---

<a id="item-3"></a>
## [macOS kernel bug causes network failure after 49.7 days of uptime, requiring reboot](https://www.tomshardware.com/software/macos/macos-has-a-49-7-day-networking-time-bomb-built-in-that-only-a-reboot-fixes-comparison-operation-on-unreliable-time-value-stops-machines-dead-in-their-tracks) ⭐️ 7.0/10

A bug in the macOS XNU kernel causes the TCP/IP networking stack to fail after approximately 49 days, 17 hours, 2 minutes, and 47 seconds of continuous system uptime. The issue stems from a 32-bit unsigned integer timer (`tcp_now`) overflowing, which violates RFC 7323 specifications and prevents the cleanup of closed TCP connections, eventually exhausting available temporary ports. This is a significant 'time-bomb' style kernel-level bug that primarily affects macOS servers, long-running workstations, or any system that remains powered on for extended periods without a reboot. It highlights a critical flaw in a core networking component that can lead to complete network unavailability, impacting services, remote access, and system reliability. The bug is located in the `tcp_now` variable within the XNU kernel's TCP stack. While existing connections may persist, new connections cannot be established after the timer overflow. The only current mitigation is a full system reboot, though researchers are investigating alternative fixes.

telegram · zaihuapd · Apr 9, 12:16

**Background**: The `tcp_now` timer is a kernel-internal clock for the TCP stack that tracks milliseconds since boot using a 32-bit unsigned integer. Such integers have a maximum value of 4,294,967,295, which when counting milliseconds, equates to roughly 49.7 days before it overflows (wraps around to zero). RFC 7323 defines extensions for high-performance TCP and includes specifications for handling such timestamp wrap-around scenarios to maintain protocol stability.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.biggo.com/news/202604080424_macos-tcp-ip-crash-49-days-uptime-bug">macOS TCP/IP Stack Crashes After 49.7 Days of Uptime Due to Kernel Timer Bug — BigGo Finance</a></li>
<li><a href="https://mjtsai.com/blog/2026/04/07/tahoe-tcp-overflow-bug/">Michael Tsai - Blog - Tahoe TCP Overflow Bug</a></li>
<li><a href="http://www.faqs.org/rfcs/rfc7323.html">RFC 7323 - TCP Extensions for High Performance ( RFC 7323 )</a></li>

</ul>
</details>

**Tags**: `#macOS`, `#Networking`, `#Kernel`, `#Security`, `#TCP/IP`

---

<a id="item-4"></a>
## [OpenAI launches $100/month ChatGPT Pro tier with 5x Plus usage limits](https://help.openai.com/en/articles/9793128-about-chatgpt-pro-plans) ⭐️ 7.0/10

OpenAI has expanded its ChatGPT Pro subscription offerings by introducing a new $100 per month tier, which provides 5 times the usage limits of the $20/month Plus plan and includes a temporary 10x Codex usage limit. The existing $200/month Pro plan, offering 20x usage limits, remains available for high-intensity parallel project workflows. This pricing update significantly lowers the entry barrier for power users who require high-volume AI interactions, making advanced features like GPT-5 and Deep Research more accessible. It represents a strategic shift in OpenAI's product lineup, offering a more granular pricing model that could attract a broader segment of professional and heavy individual users. All Pro plans include access to advanced features like GPT-5, Deep Research, Codex, image creation, and file uploads. The subscription is currently billed monthly with no annual option, and some iPhone users may need to manually select the $100 plan through their iOS Apple Account subscription settings if it's not displayed.

telegram · zaihuapd · Apr 10, 00:35

**Background**: ChatGPT usage is governed by tiered limits that restrict message frequency. The free plan has strict caps, while paid plans like Plus offer higher limits. Codex is OpenAI's model for code generation and understanding, and its usage is also subject to rate limits within subscriptions. Deep Research is an AI agent within ChatGPT that autonomously browses the web and synthesizes information to create comprehensive, cited reports on user-specified topics.

<details><summary>References</summary>
<ul>
<li><a href="https://help.openai.com/en/articles/9793128-what-is-chatgpt-pro">About ChatGPT Pro plans | OpenAI Help Center</a></li>
<li><a href="https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan">Using Codex with your ChatGPT plan | OpenAI Help Center</a></li>
<li><a href="https://openai.com/index/introducing-deep-research/">Introducing deep research | OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#ChatGPT`, `#AI Pricing`, `#Subscription Models`, `#Product Updates`

---