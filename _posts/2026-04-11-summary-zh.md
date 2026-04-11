---
layout: default
title: "Horizon Summary: 2026-04-11 (ZH)"
date: 2026-04-11
lang: zh
---

> From 17 items, 2 important content pieces were selected

---

1. [Artemis II 今日溅落太平洋，完成 50 年来首次载人绕月任务](#item-1) ⭐️ 9.0/10
2. [谷歌在 Chrome for Windows 中引入设备绑定会话凭据 (DBSC) 以应对 Cookie 窃取](#item-2) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Artemis II 今日溅落太平洋，完成 50 年来首次载人绕月任务](https://www.nasa.gov/blogs/missions/2026/04/10/artemis-ii-flight-day-10-crew-sets-for-final-burn-splashdown/) ⭐️ 9.0/10

NASA 的 Artemis II 任务于北京时间 4 月 10 日上午 8:07 在圣地亚哥海岸外的太平洋海域成功溅落，四名宇航员安全返回。这标志着自 1972 年阿波罗计划结束后，人类首次完成的载人绕月飞行任务。 此次任务是 NASA 阿尔忒弥斯计划（Artemis program）的一个关键里程碑，验证了太空发射系统（SLS）火箭和猎户座飞船（Orion）执行载人深空飞行的能力。它的成功为旨在将宇航员送上月球表面并建立可持续月球驻留的 Artemis III 任务铺平了道路。 由 NASA 宇航员 Reid Wiseman、Victor Glover、Christina Koch 和加拿大航天局宇航员 Jeremy Hansen 组成的乘组，在再入过程中经历了约 3000 华氏度的高温、计划中约 6 分钟的通信中断以及最高 3.9G 的过载。该任务于 4 月 1 日发射，总航程达 69.4 万英里。

telegram · zaihuapd · Apr 11, 00:54

**背景**: Artemis II 是 NASA 阿尔忒弥斯计划（Artemis program）的首次载人任务，该计划旨在让人类重返月球并最终前往火星。任务使用了 NASA 最强大的火箭——太空发射系统（SLS）和猎户座（Orion）载人舱。继无人测试飞行 Artemis I 之后，此次任务的一个关键目标是测试猎户座飞船在深空的生命支持系统和乘组操作。任务遵循了绕月的自由返回轨道，即利用月球引力将飞船弹射回地球，而无需进行重大的推进机动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Artemis_II">Artemis II - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artemis_program">Artemis program - Wikipedia</a></li>
<li><a href="https://www.nasa.gov/missions/nasa-answers-your-most-pressing-artemis-ii-questions/">NASA Answers Your Most Pressing Artemis II Questions - NASA</a></li>

</ul>
</details>

**标签**: `#space-exploration`, `#nasa`, `#artemis-program`, `#human-spaceflight`, `#lunar-mission`

---

<a id="item-2"></a>
## [谷歌在 Chrome for Windows 中引入设备绑定会话凭据 (DBSC) 以应对 Cookie 窃取](https://security.googleblog.com/2026/04/protecting-cookies-with-device-bound.html) ⭐️ 7.0/10

谷歌已在 Chrome 浏览器 Windows 版 146 更新中正式推出“设备绑定会话凭据”(DBSC) 功能。该技术通过硬件安全模块（如 TPM）生成一个本地存储且无法导出的密钥对，从而将用户的身份验证会话加密绑定到其物理设备上。 这是 Web 安全领域的一项重要进展，因为它直接解决了 Cookie 窃取这一根本性漏洞，而 Cookie 窃取是会话劫持攻击的主要手段。通过使被盗的 Cookie 在其他任何设备上都无法使用，DBSC 可以大幅减少账户接管事件，为用户在线账户提供更强的保护。 DBSC 协议要求浏览器在身份验证期间向 Web 服务器证明其拥有安全存储在设备上（例如在 TPM 中）的私钥。需要注意的是，此初始发布版本专门针对 Windows 版 Chrome，利用了现代 PC 上 TPM 的广泛普及性。

telegram · zaihuapd · Apr 11, 00:18

**背景**: 传统的 Web 会话依赖于存储在浏览器中的 Cookie。如果这些 Cookie 被盗（例如通过恶意软件或网络钓鱼），攻击者就可以在另一台设备上冒充用户，这种技术被称为会话劫持。可信平台模块 (TPM) 是计算机上的专用硬件芯片，可以安全地生成和存储加密密钥，防止它们被软件提取。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://w3c.github.io/webappsec-dbsc/">Device Bound Session Credentials</a></li>
<li><a href="https://en.wikipedia.org/wiki/Trusted_Platform_Module">Trusted Platform Module - Wikipedia</a></li>
<li><a href="https://owasp.org/www-community/attacks/Session_hijacking_attack">Session hijacking attack | OWASP Foundation</a></li>

</ul>
</details>

**标签**: `#Web Security`, `#Browser`, `#Authentication`, `#Cryptography`, `#Google`

---