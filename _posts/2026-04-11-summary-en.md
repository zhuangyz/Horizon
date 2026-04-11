---
layout: default
title: "Horizon Summary: 2026-04-11 (EN)"
date: 2026-04-11
lang: en
---

> From 17 items, 2 important content pieces were selected

---

1. [Artemis II Splashes Down in Pacific, Completing First Crewed Lunar Orbit Mission in 50 Years](#item-1) ⭐️ 9.0/10
2. [Google introduces Device-Bound Session Credentials (DBSC) in Chrome for Windows to combat cookie theft](#item-2) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Artemis II Splashes Down in Pacific, Completing First Crewed Lunar Orbit Mission in 50 Years](https://www.nasa.gov/blogs/missions/2026/04/10/artemis-ii-flight-day-10-crew-sets-for-final-burn-splashdown/) ⭐️ 9.0/10

NASA's Artemis II mission, carrying four astronauts, successfully splashed down in the Pacific Ocean off the coast of San Diego at 8:07 AM Beijing Time on April 10, 2026. This event marks the completion of humanity's first crewed mission to orbit the Moon since the Apollo program ended in 1972. This mission is a critical milestone for NASA's Artemis program, demonstrating the capabilities of the Space Launch System (SLS) rocket and Orion spacecraft for crewed deep-space travel. Its success paves the way for Artemis III, which aims to land astronauts on the lunar surface and establish a sustainable human presence on the Moon. The crew, consisting of NASA astronauts Reid Wiseman, Victor Glover, Christina Koch, and Canadian Space Agency astronaut Jeremy Hansen, endured a re-entry with temperatures around 3,000°F, a planned 6-minute communications blackout, and peak G-forces of 3.9. The mission, launched on April 1, traveled a total distance of 694,000 miles.

telegram · zaihuapd · Apr 11, 00:54

**Background**: Artemis II is the first crewed mission of NASA's Artemis program, which aims to return humans to the Moon and eventually send them to Mars. The mission utilized the Space Launch System (SLS), NASA's most powerful rocket, and the Orion crew capsule. A key objective was to test Orion's life support systems and crew operations in deep space, following the uncrewed Artemis I test flight. The mission followed a free-return trajectory around the Moon, a path that uses lunar gravity to slingshot the spacecraft back to Earth without major propulsion maneuvers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Artemis_II">Artemis II - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artemis_program">Artemis program - Wikipedia</a></li>
<li><a href="https://www.nasa.gov/missions/nasa-answers-your-most-pressing-artemis-ii-questions/">NASA Answers Your Most Pressing Artemis II Questions - NASA</a></li>

</ul>
</details>

**Tags**: `#space-exploration`, `#nasa`, `#artemis-program`, `#human-spaceflight`, `#lunar-mission`

---

<a id="item-2"></a>
## [Google introduces Device-Bound Session Credentials (DBSC) in Chrome for Windows to combat cookie theft](https://security.googleblog.com/2026/04/protecting-cookies-with-device-bound.html) ⭐️ 7.0/10

Google has officially launched Device-Bound Session Credentials (DBSC) in Chrome version 146 for Windows. This technology cryptographically binds a user's authentication session to their physical device by using a hardware security module, like a TPM, to generate a key pair that is stored locally and cannot be exported. This is a significant advancement in web security as it directly addresses the fundamental vulnerability of cookie theft, which is a primary method for session hijacking attacks. By making stolen cookies useless on any other machine, DBSC can drastically reduce account takeover incidents, providing stronger protection for users' online accounts. The DBSC protocol requires the browser to prove possession of a private key securely stored on the device (e.g., in a TPM) to the web server during authentication. It's important to note that this initial rollout is specifically for Chrome on Windows, leveraging the widespread availability of TPMs on modern PCs.

telegram · zaihuapd · Apr 11, 00:18

**Background**: Traditional web sessions rely on cookies stored in the browser. If these cookies are stolen (e.g., via malware or phishing), an attacker can impersonate the user on another device, a technique known as session hijacking. A Trusted Platform Module (TPM) is a dedicated hardware chip on a computer that can securely generate and store cryptographic keys, preventing them from being extracted by software.

<details><summary>References</summary>
<ul>
<li><a href="https://w3c.github.io/webappsec-dbsc/">Device Bound Session Credentials</a></li>
<li><a href="https://en.wikipedia.org/wiki/Trusted_Platform_Module">Trusted Platform Module - Wikipedia</a></li>
<li><a href="https://owasp.org/www-community/attacks/Session_hijacking_attack">Session hijacking attack | OWASP Foundation</a></li>

</ul>
</details>

**Tags**: `#Web Security`, `#Browser`, `#Authentication`, `#Cryptography`, `#Google`

---