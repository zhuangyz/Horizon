---
layout: default
title: "Horizon Summary: 2026-04-14 (EN)"
date: 2026-04-14
lang: en
---

> From 23 items, 7 important content pieces were selected

---

1. [Backblaze quietly changed backup policy, excluding cloud storage folders without user notification.](#item-1) ⭐️ 8.0/10
2. [Steve Yegge Claims Google's AI Adoption Mirrors Traditional Industries Like John Deere](#item-2) ⭐️ 8.0/10
3. [Major Media Outlets Block Internet Archive's Crawler, Journalists Rally for Digital Preservation](#item-3) ⭐️ 8.0/10
4. [Stanford's 2026 AI Index Report: US-China AI Performance Gap Nearly Closed, Adoption Accelerates](#item-4) ⭐️ 8.0/10
5. [Jujutsu (jj) CLI tool introduces automatic committing and a new mental model for version control](#item-5) ⭐️ 7.0/10
6. [Blackmagic Design Releases DaVinci Resolve Photo, Bringing Video Color Tools to Still Images](#item-6) ⭐️ 7.0/10
7. [Google Announces New Spam Policy Targeting 'Back Button Hijacking'](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Backblaze quietly changed backup policy, excluding cloud storage folders without user notification.](https://rareese.com/posts/backblaze/) ⭐️ 8.0/10

Backblaze updated its backup client to automatically exclude folders from popular cloud storage providers like OneDrive, Google Drive, and Dropbox from its backup sets. This policy change was implemented without direct notification to users, potentially leading to data loss for those who relied on Backblaze to back up files stored in these synchronized directories. This change undermines user trust in a major backup service and highlights the risks of relying on 'unlimited' consumer SaaS products with opaque policy shifts. It forces a reevaluation of backup strategies, especially for users who treat cloud-synced folders as part of their local data ecosystem and assumed they were protected. The exclusion targets both mount points and cache directories for services including Box, iDrive, and others, officially to prevent performance issues and excessive data usage. However, the change was not prominently communicated, and the standard Backblaze Personal backup plan has a 30-day version history limit by default, which can compound data loss if files are deleted or overwritten in a cloud folder after the exclusion takes effect.

hackernews · rrreese · Apr 14, 08:30

**Background**: Backblaze is a popular cloud backup service known for its 'unlimited' backup plan for personal computers. Many users employ services like Dropbox or OneDrive to sync files across devices, creating local folders that appear as regular directories. Traditionally, backup software like Backblaze would include these local sync folders in its backup set, providing a second copy of cloud-stored data. The 3-2-1 backup rule recommends having at least three copies of data, on two different media, with one copy off-site.

<details><summary>References</summary>
<ul>
<li><a href="https://rareese.com/posts/backblaze/">Backblaze has quietly stopped backing up your data | Robert Reese's Website</a></li>
<li><a href="https://www.backblaze.com/computer-backup/docs/backup-client-release-notes-windows">Backup Client Release Notes (Windows)</a></li>
<li><a href="https://www.backblaze.com/computer-backup/docs/supported-backup-data">Supported Backup Data</a></li>

</ul>
</details>

**Discussion**: The community expressed significant frustration over the lack of notification and perceived breach of trust, with users reporting actual data loss. Discussions highlighted tensions around Backblaze's 'unlimited' business model for personal use, its positioning as a consumer versus professional tool, and technical challenges like backing up cloud storage with 'Files On-Demand' features that could exhaust local disk space.

**Tags**: `#backup`, `#cloud-storage`, `#data-loss`, `#policy-change`, `#saas`

---

<a id="item-2"></a>
## [Steve Yegge Claims Google's AI Adoption Mirrors Traditional Industries Like John Deere](https://simonwillison.net/2026/Apr/13/steve-yegge/#atom-everything) ⭐️ 8.0/10

Former Google engineer Steve Yegge reported, based on a conversation with a long-time Google tech director, that Google's internal AI adoption curve is surprisingly similar to that of traditional companies like tractor manufacturer John Deere, with only about 20% being 'agentic power users'. This observation was immediately contested by Google executives Addy Osmani and Demis Hassabis, who called the claims false and cited widespread internal use of AI tools. This public disagreement highlights a critical debate about the real pace of AI integration within even the most advanced tech companies. If a leader like Google faces adoption challenges similar to non-tech industries, it suggests that organizational and cultural barriers to AI may be universal, potentially slowing industry-wide innovation. Yegge described a common industry adoption pattern of 20% agentic power users, 20% outright refusers, and 60% still using basic chat tools like Cursor. He also linked perceived organizational stagnation to an 18-month industry-wide hiring freeze, which he claims has limited the influx of fresh external perspectives. In contrast, Addy Osmani stated that over 40,000 Google software engineers use agentic coding weekly, with access to a suite of custom AI tools and systems.

rss · Simon Willison · Apr 13, 20:59

**Background**: Steve Yegge is a well-known software engineer and blogger famous for his critical analyses of tech giants, having worked at both Amazon and Google. 'Agentic AI' refers to AI systems that can autonomously perform tasks and make decisions to achieve goals, beyond just providing suggestions. Cursor is an AI-powered integrated development environment (IDE) that many developers use for coding assistance through a chat interface. The tech industry has experienced significant hiring freezes since late 2024, aimed at cost-cutting but often criticized for impacting innovation and knowledge flow.

<details><summary>References</summary>
<ul>
<li><a href="https://www.grammarly.com/agentic-ai">What is Agentic AI ? | Agentic AI 101</a></li>
<li><a href="https://cursor.com/">Cursor : The best way to code with AI</a></li>
<li><a href="https://suchwork.org/hiring-freeze/">Hiring Freeze: Navigating the Impact on Workforce Strategy – SuchWork</a></li>

</ul>
</details>

**Discussion**: The discussion, as reflected in the quoted executive responses, is highly polarized. Yegge's insider critique presents a narrative of surprising conformity and potential mediocrity. Google's official rebuttal, from figures like Osmani and Hassabis, strongly denies this characterization, asserting robust internal AI adoption and labeling the original post as 'nonsense' and 'clickbait.' This creates a stark 'he said, they said' dynamic about the true state of AI at Google.

**Tags**: `#AI Adoption`, `#Google`, `#Organizational Culture`, `#Software Engineering`, `#Industry Trends`

---

<a id="item-3"></a>
## [Major Media Outlets Block Internet Archive's Crawler, Journalists Rally for Digital Preservation](https://www.wired.com/story/the-internets-most-powerful-archiving-tool-is-in-mortal-peril/) ⭐️ 8.0/10

At least 23 major news outlets and platforms, including The New York Times, Gannett (parent of USA Today), and Reddit, have begun blocking the Internet Archive's 'ia_archiverbot' crawler, primarily over concerns that archived content is being used to train AI models. In response, over 100 journalists have signed an open letter organized by the Electronic Frontier Foundation (EFF) defending the archive's critical role in fact-checking and preserving historical records. This conflict represents a critical juncture where the imperatives of AI development, copyright enforcement, and digital preservation are clashing directly. The outcome could significantly weaken public access to a historical record of the web, impacting journalism, research, and accountability, while setting a precedent for how web crawlers essential for public archives are treated. The blocking is implemented via the robots.txt protocol, targeting the specific user-agent 'ia_archiver'. Some outlets, like The Guardian, have taken a more nuanced approach by restricting API access instead of a full block. The Internet Archive has warned that such blocks on the public web severely undermine society's ability to understand history and current events.

telegram · zaihuapd · Apr 14, 00:12

**Background**: The Internet Archive is a non-profit digital library best known for its Wayback Machine, which archives snapshots of publicly accessible web pages over time. Its automated web crawler, identified by the user-agent 'ia_archiver', systematically collects these snapshots in a process known as web archiving. The Electronic Frontier Foundation (EFF) is a leading non-profit digital rights organization that advocates for civil liberties in the digital world.

<details><summary>References</summary>
<ul>
<li><a href="https://datadome.co/bots/internet-archive/">What is Internet Archive crawler bot</a></li>
<li><a href="https://en.wikipedia.org/wiki/Web_archiving">Web archiving - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Electronic_Frontier_Foundation">Electronic Frontier Foundation - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI Ethics`, `#Digital Preservation`, `#Copyright`, `#Web Archiving`, `#Media`

---

<a id="item-4"></a>
## [Stanford's 2026 AI Index Report: US-China AI Performance Gap Nearly Closed, Adoption Accelerates](https://hai.stanford.edu/ai-index/2026-ai-index-report) ⭐️ 8.0/10

Stanford University's 2026 AI Index Report reveals that the performance gap between US and Chinese AI models has nearly vanished, with the US lead held by Anthropic now at just 2.7%. The report also shows China leading globally in several metrics, including AI research papers, patents, industrial robot installations, and public AI supercomputers, while global AI adoption is accelerating with significant workforce impacts. This report provides critical evidence of China's rapid catch-up in AI capabilities, potentially reshaping the global technological balance of power and intensifying US-China competition. The accelerating global AI adoption and its documented impact on software developer jobs highlight the urgent need for workforce adaptation strategies and policy responses worldwide. The report notes that while over 90% of top AI models now excel in multiple human benchmarks, they exhibit a 'jagged frontier' phenomenon where capabilities are uneven across different tasks. Additionally, global AI computing power has grown 30-fold in three years, and corporate investment has doubled to $581.7 billion, while the number of AI researchers entering the US has plummeted by 80% in the past year.

telegram · zaihuapd · Apr 14, 05:09

**Background**: The AI Index Report is an annual publication from Stanford University's Institute for Human-Centered Artificial Intelligence (HAI) that tracks, collates, and visualizes data on artificial intelligence development globally. Anthropic is an American AI safety and research company known for developing large language models like Claude. The 'jagged frontier' refers to the phenomenon where AI models perform exceptionally well on some tasks while struggling with others that might seem similar in difficulty to humans, highlighting the uneven nature of current AI capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-index/2025-ai-index-report">The 2025 AI Index Report | Stanford HAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI Research`, `#Global AI Trends`, `#Technology Policy`, `#AI Workforce`, `#Industry Analysis`

---

<a id="item-5"></a>
## [Jujutsu (jj) CLI tool introduces automatic committing and a new mental model for version control](https://steveklabnik.github.io/jujutsu-tutorial/introduction/what-is-jj-and-why-should-i-care.html) ⭐️ 7.0/10

Jujutsu (jj), a new command-line version control tool, has been released with a fundamentally different workflow from Git, featuring automatic committing of all changes and eliminating the traditional staging area. It maintains full compatibility with existing Git repositories, allowing developers to use it transparently alongside teammates who continue using Git. This matters because it challenges the dominant Git paradigm by reducing cognitive overhead and making version control operations more fluid and less error-prone. If widely adopted, it could significantly change developer workflows, especially for those dealing with complex branching, frequent context switching, or merge conflicts, potentially increasing productivity. A key technical detail is that jj automatically creates a commit for every change to the working copy, which fundamentally alters the edit-commit workflow. While this enables powerful undo operations and conflict handling, it requires users to adopt a defensive practice of creating empty commits when they need to examine an old state without altering history.

hackernews · tigerlily · Apr 14, 10:33

**Background**: Git is the dominant distributed version control system (DVCS), using a model where developers explicitly stage changes before committing them to a local history. The staging area (or index) is a core Git concept that separates modified files from committed snapshots. Jujutsu (jj) is a newer DVCS that uses Git as a backend storage layer but presents a different, change-centric interface to users, aiming to simplify common operations.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.jj-vcs.dev/latest/">Jujutsu—a version control system - docs.jj-vcs.dev</a></li>
<li><a href="https://docs.jj-vcs.dev/latest/git-comparison/">Git comparison - Jujutsu docs</a></li>
<li><a href="https://github.com/jj-vcs/jj/blob/main/docs/git-comparison.md">jj/docs/git-comparison.md at main · jj-vcs/jj · GitHub</a></li>

</ul>
</details>

**Discussion**: The community discussion reveals mixed but thoughtful reactions. Some users are actively comparing jj with other modern tools like GitButler and exploring its paradigm shift. Key concerns include the need to adjust to the automatic committing model, with one user noting it requires creating empty commits to safely examine old code. Another user expresses skepticism about adoption, citing the difficulty of displacing an industry standard like Git without a platform like GitHub driving it.

**Tags**: `#version-control`, `#developer-tools`, `#git`, `#cli`, `#workflow`

---

<a id="item-6"></a>
## [Blackmagic Design Releases DaVinci Resolve Photo, Bringing Video Color Tools to Still Images](https://www.blackmagicdesign.com/products/davinciresolve/photo) ⭐️ 7.0/10

Blackmagic Design has released DaVinci Resolve Photo, a new standalone photo editing application that brings professional video color grading tools and native RAW support for Canon, Fujifilm, Nikon, Sony, and iPhone ProRAW files to still photography workflows. This release is significant because it bridges the gap between professional video and photo editing, offering photographers access to DaVinci Resolve's industry-leading color science and grading tools previously reserved for video post-production. It introduces new competition in the professional photo editing market, potentially challenging established players like Adobe. The application includes native RAW support for major camera brands and iPhone ProRAW, and it inherits advanced features from DaVinci Resolve such as HDR grading, face retouching, and noise reduction. However, some users report that the Linux version can be difficult to set up, and detailed technical specifications are not prominently listed on the product page.

hackernews · thebiblelover7 · Apr 14, 02:25

**Background**: DaVinci Resolve is a professional video editing, color correction, and audio post-production software suite developed by Blackmagic Design, widely used in film and television for its powerful color grading capabilities. RAW files are unprocessed image data captured by a camera sensor, offering greater flexibility in editing compared to compressed formats like JPEG. The photo editing software market has been dominated by tools like Adobe Lightroom and Photoshop, with open-source alternatives like Darktable pushing technical innovation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.blackmagicdesign.com/products/davinciresolve/color">DaVinci Resolve – Color | Blackmagic Design</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blackmagic_Design">Blackmagic Design - Wikipedia</a></li>
<li><a href="https://petapixel.com/best-free-raw-editing-programs/">The Best Free RAW Photo Editing Programs in 2026 - PetaPixel</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive and excited about the potential of professional video color tools for photography. Key discussion points include enthusiasm for the feature set, frustration over Linux installation difficulties and lack of clear technical specs, and comparisons to existing tools like Darktable. Some users expressed that this release fulfilled a long-standing wish for a DaVinci Resolve-based photo editor.

**Tags**: `#photo-editing`, `#davinci-resolve`, `#raw-processing`, `#creative-tools`, `#software-release`

---

<a id="item-7"></a>
## [Google Announces New Spam Policy Targeting 'Back Button Hijacking'](https://developers.google.com/search/blog/2026/04/back-button-hijacking) ⭐️ 7.0/10

Google has announced a new spam policy specifically targeting 'back button hijacking,' a technique where websites manipulate browser history to prevent users from easily navigating away. The policy aims to classify such manipulative practices as spam and potentially penalize offending sites in search rankings. This matters because back button hijacking severely degrades user experience and can be used for deceptive or malicious purposes, such as trapping users on ad-filled pages or facilitating phishing attacks. By taking action, Google is addressing a widespread web annoyance and aligning its search quality efforts with core user experience principles. The policy enforcement will rely on Google's detection systems to identify sites that use techniques like `history.replaceState` or `location.replace` to manipulate the browser's history stack without user consent. Notably, the community discussion highlights that major platforms like LinkedIn and Microsoft have been cited as real-world examples of this practice.

hackernews · zdw · Apr 14, 03:06

**Background**: Back button hijacking is a manipulative web practice where JavaScript or other techniques are used to interfere with the normal functioning of a browser's back button. Normally, clicking 'back' should return the user to the previous page in their browsing history. However, hijacking can redirect users to unwanted pages, keep them on the same site, or even facilitate attacks by exploiting referrer information. Google's web spam policies are designed to combat various tactics that manipulate search results or degrade user experience for unfair gain.

<details><summary>References</summary>
<ul>
<li><a href="https://wolf-of-seo.de/en/what-is/back-button-hijack/">What is Back Button Hijack ? A glossary entry about online risks</a></li>
<li><a href="https://chromium.googlesource.com/chromium/src/+/main/docs/history_manipulation_intervention.md">Chromium Docs - History manipulation intervention in Chromium</a></li>

</ul>
</details>

**Discussion**: The community reaction is largely positive but skeptical about enforcement, with users hoping Google can make it work effectively. Commenters provided specific examples of major platforms like LinkedIn and Microsoft engaging in this practice, validating the problem's significance. Some users expressed a desire for even broader protection, arguing against any form of back-button interference, not just spam-related hijacking.

**Tags**: `#web-development`, `#user-experience`, `#search-engines`, `#browser-security`, `#spam-policy`

---