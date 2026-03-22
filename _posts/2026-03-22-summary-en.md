---
layout: default
title: "Horizon Summary: 2026-03-22 (EN)"
date: 2026-03-22
lang: en
---

> From 14 items, 3 important content pieces were selected

---

1. [Elon Musk plans to deploy AI computing centers in space within 30-36 months.](#item-1) ⭐️ 8.0/10
2. [Simon Willison demonstrates AI-powered user profiling using Hacker News comment history](#item-2) ⭐️ 7.0/10
3. [Unitree plans 20,000 humanoid robots by 2026, targets home market to challenge Tesla's Optimus](#item-3) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Elon Musk plans to deploy AI computing centers in space within 30-36 months.](https://t.me/zaihuapd/40437) ⭐️ 8.0/10

Elon Musk announced plans to deploy AI computing centers in space within 30 to 36 months, citing superior solar efficiency as a solution to Earth's energy constraints for AI growth. He also detailed related initiatives including a goal to produce 100 GW of solar cells annually through Tesla and SpaceX, the construction of a massive chip factory called TeraFab, and an annual production target of 1 million units for the Optimus Gen 3 humanoid robot. This announcement is significant as it proposes a radical solution to the critical bottleneck of energy supply for the exponential growth of AI, potentially decoupling compute capacity from terrestrial power grids. If realized, it could reshape the economics and geography of high-performance computing, while the integrated vision for solar, chip manufacturing, and robotics aims to create a vertically-scaled ecosystem for automation and AI. Musk claims space offers 5 times the solar efficiency of Earth and eliminates the need for battery storage. The TeraFab chip factory, a joint Tesla-SpaceX project, is designed to produce over one terawatt of AI compute capacity per year. The Optimus Gen 3 robot features hands with 22 degrees of freedom, a significant upgrade aimed at general-purpose tasks.

telegram · zaihuapd · Mar 22, 02:24

**Background**: Space-based solar power is a concept where solar energy is collected in space and transmitted to Earth, offering advantages like nearly continuous sunlight (up to 99.9% of the time in geosynchronous orbit) compared to terrestrial panels limited by day-night cycles and weather. TeraFab is a proposed large-scale semiconductor fabrication project by Tesla and SpaceX targeting massive AI compute chip production. Tesla's Optimus is a humanoid robot project intended for tasks deemed dangerous, repetitive, or boring, with its development progressing through generations featuring improved dexterity, such as the Gen 3's 22-DOF hands.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Space-based_solar_power">Space-based solar power - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Terafab">Terafab - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Optimus_(robot)">Optimus (robot) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI Infrastructure`, `#Space Technology`, `#Renewable Energy`, `#High-Performance Computing`, `#Strategic Vision`

---

<a id="item-2"></a>
## [Simon Willison demonstrates AI-powered user profiling using Hacker News comment history](https://simonwillison.net/2026/Mar/21/profiling-hacker-news-users/#atom-everything) ⭐️ 7.0/10

Simon Willison has developed and described a method to profile Hacker News users by programmatically fetching their last 1,000 comments via the Algolia API and then analyzing the aggregated text with a large language model like Claude Opus. He created a simple web tool that uses the API's open CORS headers to fetch comment data for any username and provides a convenient copy-to-clipboard function for the LLM analysis step. This technique demonstrates how publicly accessible social data, combined with modern AI, can be used to infer detailed personal and professional profiles, raising significant privacy and ethical questions for online communities. It also showcases a practical, low-code application of LLMs for social data analysis, potentially influencing how researchers, marketers, or community managers approach public forum data. The method relies on the Algolia Hacker News API endpoint `search_by_date`, which allows filtering comments by the `author_username` tag and supports fetching up to 1,000 hits per request. A key technical enabler is that the API is served with open CORS headers, allowing the fetching tool to run client-side JavaScript from any webpage without server-side proxying.

rss · Simon Willison · Mar 21, 23:59

**Background**: Hacker News is a popular social news website focused on technology and entrepreneurship, run by the startup incubator Y Combinator. The Algolia Hacker News API is a free, public API that provides full-text search over Hacker News content, including stories and comments, without requiring authentication. CORS (Cross-Origin Resource Sharing) headers are HTTP headers that tell a browser to allow a web application running at one origin to access resources from a different origin, which is why Simon's tool can fetch data directly from a user's browser.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@otabekjon0302/how-to-use-a-hacker-news-data-from-algolia-api-d7dd32341436">How to Use a Hacker News data from Algolia API | by Otabekjon | Medium</a></li>
<li><a href="https://stackoverflow.com/questions/50261027/access-algolia-rest-api-via-javascript-cors-errors">Access Algolia REST API via JavaScript: CORS errors - Stack Overflow</a></li>

</ul>
</details>

**Tags**: `#data-analysis`, `#hacker-news`, `#api`, `#llm`, `#profiling`

---

<a id="item-3"></a>
## [Unitree plans 20,000 humanoid robots by 2026, targets home market to challenge Tesla's Optimus](https://www.eweek.com/news/unitree-20000-humanoid-robots-2026-china/) ⭐️ 7.0/10

Chinese robotics company Unitree plans to scale its humanoid robot production to 20,000 units by 2026, a significant increase from its 2025 target of about 5,500 units. The company is also preparing for a Shanghai IPO to raise 4.2 billion yuan for platform development and intends to enter the home robot market within three years, directly competing with Tesla's Optimus. This announcement signals a major acceleration in the commercialization of humanoid robots, with Unitree aiming to capture a significant share of a market where Chinese manufacturers already dominate nearly 80% of global shipments. The direct competition with Tesla in the consumer space could drive faster innovation, lower costs, and broader adoption of humanoid robotics technology. According to Morgan Stanley data, global humanoid robot shipments in 2025 are projected to be around 13,000 units, with Unitree and another Chinese firm, Zhiyuan Robotics, being the primary contributors to China's dominant market share. Unitree's H2 humanoid robot features 31 degrees of freedom and integrated voice interaction, designed for practical deployment and research applications.

telegram · zaihuapd · Mar 22, 04:15

**Background**: Unitree Robotics is a leading Chinese company known initially for its high-performance quadrupedal (dog-like) robots, which have been featured in high-profile events like the CCTV Spring Festival Gala and the Winter Olympics opening ceremony. Humanoid robots, like Tesla's Optimus and Unitree's H2, are bipedal machines designed to perform tasks in human environments, representing a frontier in robotics focused on general-purpose automation. The competition in this space involves significant technical challenges in locomotion, manipulation, and AI integration, with companies aiming to move from research prototypes to mass-produced, commercially viable products.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unitree.com/">Unitree Robotics | Robot Dog_Quadruped_Humanoid Robotics Company</a></li>
<li><a href="https://www.reuters.com/world/asia-pacific/unitree-plans-shanghai-ipo-testing-interest-humanoid-robots-2026-03-20/">Unitree plans Shanghai IPO, testing interest in humanoid robots</a></li>
<li><a href="https://en.wikipedia.org/wiki/Optimus_(robot)">Optimus (robot) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#humanoid-robots`, `#industrial-news`, `#china-tech`, `#tesla-competition`

---