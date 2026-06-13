# 🎯 Bounty Domains Scraper v1.0

[![GitHub Pages Deployment](https://img.shields.io/badge/Live_Demo-Hosted_on_GitHub-emerald?style=for-the-badge&logo=githubpages&logoColor=white)](https://santhoshkumarkuppan.github.io/Domains-With-Bounty/)
[![Automated Pipeline](https://img.shields.io/badge/Pipeline-GitHub_Actions-blue?style=for-the-badge&logo=githubactions&logoColor=white)](https://github.com/santhoshkumarkuppan/Domains-With-Bounty/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-amber.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

> An automated, single-page aggregator tracking active scopes, reward structures, and high-impact attack vectors across public bug bounty engines like HackerOne and Bugcrowd.

---

## ⚡ The Architectural Blueprint

Vuln-Tracker utilizes a **Jamstack Architecture** to ensure fast loading times and zero hosting costs. 

1. **The Backend Core (`scraper.py`)**: A Python engine orchestrated via GitHub Actions that handles target discovery, bounty ranges, and metadata extraction.
2. **The Decentralized DB (`data.json`)**: An optimized state payload rewritten entirely every 24 hours via data synchronization loops.
3. **The Glassmorphic Frontend (`index.html`)**: A lightweight dashboard styled with Tailwind CSS and powered reactive client-side filters using Alpine.js.

```text
[ GitHub Actions Cron ] ──► (Runs scraper.py) ──► [ Writes data.json ] ──► [ Hosted Page UI ]