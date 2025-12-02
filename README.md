# 🏋️‍♂️ Cybersecurity Daily Drills

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Status](https://img.shields.io/badge/Status-Daily%20Updates-success?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Muscle%20Memory-orange?style=for-the-badge)

> **"Consistency is more important than intensity."**

## 📖 About This Repository
This repository is my **Cybersecurity Gym**. While my [Main Portfolio](https://github.com/d-osei/Cybersecurity-Portfolio) contains complete, polished projects, this repository houses my daily 30-minute practice drills.

Here, I focus on building **muscle memory** for essential analyst skills: log parsing, regex, API scraping, and data visualization. The goal is to solve one specific problem every day to maintain a "Green" GitHub contribution graph and sharpen my Python scripting skills.

---

## 📅 The Training Schedule
To ensure a well-rounded skillset, I follow a thematic schedule:

| Day | Theme | Focus Area | Typical Tools |
| :--- | :--- | :--- | :--- |
| **Mon** | 🌐 **Network Traffic** | Firewall logs, Flow analysis, PCAP parsing | `Pandas`, `Wireshark` |
| **Tue** | 🔐 **Authentication** | SSH brute force, Windows Event Logs (4624/4625) | `Regex`, `Jupyter` |
| **Wed** | 🦠 **Threat Intel** | Parsing IOC feeds, checking IP reputations | `Requests`, `APIs` |
| **Thu** | 🕸️ **Web Attacks** | Apache/Nginx logs, SQLi/XSS pattern matching | `Urllib`, `Pandas` |
| **Fri** | 📊 **Visualization** | Graphing attack trends, heatmaps | `Matplotlib`, `NetworkX` |
| **Wkd** | 🧹 **Refinement** | Code cleanup, documentation, deep dives | `Git` |

---

## 📂 Repository Structure
I organize drills by date to track progression over time.

```text
2025/
├── 11-Nov/
│   ├── 2025-11-24_Apache-Log-Parse.ipynb
│   ├── 2025-11-25_SSH-Failures.ipynb
│   └── 2025-11-26_Feodo-Tracker-Check.ipynb
└── data/             # Small sample logs used for drills
    ├── auth.sample.log
    └── access.sample.log
